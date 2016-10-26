**PHPExcelReader** 是一个轻量级的excel文件读取类, 支持 CSV, XLS, XLSX 文件

### 依赖:
*  PHP 5.3.0+
*  PHP 必须开启支持Zip文件处理 (see http://php.net/manual/en/zip.installation.php)

### 例子:


	<?php
		use writethesky\PHPExcelReader\PHPExcelReader;

		$Reader = new PHPExcelReader('test.xls');
		$total = $Reader->count();			// 获取总行数
		//$current = $Reader->current();	// 获取当前行数据

		/*
		$Reader->seek(4);					// 跳到第4行
		$row = $Reader->current();			// 获取当前行数据
		*/

		/*
		foreach($Reader as $key => $row){
			$data[] = $row;					// 循环行内数据
		}
		*/

		var_dump($total);
		

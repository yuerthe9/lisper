LISPER
======
-------
##一：基础知识 - The basics
* 从一个实例开始  
  将下列代码保存为hello-world.lisp，一个基于restas的简单web应用程序。
  ```
   ;;;; hello-world.lisp 
    (ql:quickload "restas") 
	 
	 (restas:define-module #:hello-world
	       (:use :cl :restas))
	  
	  (in-package #:hello-world)
	 
	 (define-route hello-world ("")
	     "Hello World")
	  
	  (start '#:hello-world :port 8080)
	  ```


##小技巧
	  编码处理：
	  (load "restas-test" :external-format '(:gbk))

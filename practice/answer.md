#### 1、创建表

CREATE TABLE `class` ( `cid` VARCHAR(10) NOT NULL , `caption` VARCHAR(10) NOT NULL , PRIMARY KEY (`cid`));

CREATE TABLE `student` ( `sid` VARCHAR(10) NOT NULL , `sname` VARCHAR(10) NOT NULL , `gender` VARCHAR(10) NOT NULL , `class_id` VARCHAR(10) NOT NULL , PRIMARY KEY (`sid`));

CREATE TABLE `teacher` ( `tid` VARCHAR(10) NOT NULL , `tname` VARCHAR(10) NOT NULL , PRIMARY KEY (`tid`));

CREATE TABLE `course` ( `cid` VARCHAR(10) NOT NULL , `cname` VARCHAR(10) NOT NULL , `teach_id` VARCHAR(10) NOT NULL , PRIMARY KEY (`cid`)) ENGINE = MyISAM;

CREATE TABLE `score` ( `sid` VARCHAR(10) NOT NULL , `stu_id` VARCHAR(10) NOT NULL , `course_id` VARCHAR(10) NOT NULL , `number` VARCHAR(10) NOT NULL , PRIMARY KEY (`sid`));

插入数据

INSERT INTO `class` (`cid`, `caption`) VALUES ('1', '三年二班'), ('2', '一年三班'), ('3', '三年一班')

INSERT INTO `student` (`sid`, `sname`, `gender`, `class_id`) VALUES ('1', '钢蛋', '女', '1'), ('2', '铁锤', '女', '1'), ('3', '山炮', '男', '2')

INSERT INTO `teacher` (`tid`, `tname`) VALUES ('1', '波多'), ('2', '苍空'), ('3', '饭岛')

INSERT INTO `course` (`cid`, `cname`, `teach_id`) VALUES ('1', '生物', '1'), ('2', '体育', '1'), ('3', '物理', '2')

INSERT INTO `score` (`sid`, `stu_id`, `course_id`, `number`) VALUES ('1', '1', '1', '81'), ('2', '1', '2', '80'), ('3', '2', '2', '90')


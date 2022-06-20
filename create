create table Student
(
    `student_id` int(10) primary key auto_increment not null comment '学生id',
    `student_name` varchar(20) not null comment '学生姓名',
    `student_sex` varchar(2) not null comment '性别',
    `student_age` int(2) not null comment '年龄',
    `student_tel` int(12) not null comment '电话',
    `student_title` int(1) comment '账号状态1是封号0是没有封号'
)comment '学生表';

create table Teacher
(
    `teacher_id` int(10) primary key auto_increment not null comment '老师id',
    `teacher_name` varchar(20) not null comment '老师姓名'
)comment '老师表';

create table Class
(
    `class_id` int(10) primary key auto_increment not null comment '课程id',
    `class_name` varchar(20) not null comment '课程名字'
)comment '课程表';

create table Transcript
(
    `Transcript_id` int(10) primary key auto_increment not null comment '成绩id',
    `Transcript_name` varchar(20) not null comment '学科名字',
    `Transcript_fraction` int(6) comment '分数'
)comment '成绩表';

create table login
(
    user_id int(10) primary key not null auto_increment comment '用户id',
    username varchar(10) not null comment '用户名',
    passwd int(20) not null comment '用户密码'
) comment '登陆';

alter table Teacher add constraint studentteacher foreign key (teacher_id) references StudentManagementSystem.Student (student_id);
alter table Class add constraint classteacher foreign key (class_id) references StudentManagementSystem.Student (student_id);
alter table Transcript add constraint transcirptteacher foreign key (Transcript_id) references StudentManagementSystem.Student (student_id);
alter table login add constraint loginstudent foreign key (user_id) references StudentManagementSystem.Student (student_id);

insert into StudentManagementSystem.Student values (1,'张三','男',18,152840707,0);
insert into StudentManagementSystem.Student values (2,'张四','男',18,252840707,0);
insert into StudentManagementSystem.Teacher values (1,'杨老师');
insert into StudentManagementSystem.Teacher values (2,'张老师');
insert into StudentManagementSystem.Transcript values (1,'语文',1);
insert into StudentManagementSystem.Transcript values (2,'数学',2);
insert into StudentManagementSystem.Class values (1,'语文');
insert into StudentManagementSystem.Class values (2,'数学');
insert into StudentManagementSystem.login values (1,'root',1129491453);

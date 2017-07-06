# 常量
如const string c_helpInfo = "帮助";
# 变量
声明时一行一个变量
## 临时变量
以小写单词开始，第二个单词开始首字母大写(Camel风格)
如 bool isFinished;
## 静态变量
如 static bool s_isFinished;
## 全局变量
如 bool g_isFinished;
## 类成员变量
如 bool m_backgroundPicture;
## 特殊部分
如下标变量 可考虑在局部使用
int i;
int cnt;
# 函数
## 普通函数
## 类成员函数
以动词开始，以小写单词开始，第二个单词开始首字母大写(Camel风格)
如static cocos2d::Scene* createScene();
# 符号使用
## 关于{}
所有条件判断都要使用{}，且‘{’留在上一行，‘}’另起一行
如 if () {
}
## 换行退格
使用tab对齐 一个tab设为4空格宽度 不要使用空格

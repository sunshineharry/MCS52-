# 微机原理与接口技术课程实验

## 目录说明
- 文件夹 `01`-`05_final` 分别为实验一-实验五，其中，实验五以`05_final`为准，文件夹`05`可以无视
  
- 所有的压缩文件可以无视


## 文件说明
- `proteus`文件夹中为proteus仿真
  
- `code`文件夹中为源代码
  
    - `src`目录为所有的`.c`文件
  
    - `dependence`目录为所有的`.h`文件
  
    - 其他目录都为中间文件或配置文件

## 函数命名
- 以  `_` 开头的函数表示只在所在文件当中起作用，不对外展现接口，例如`_LCD_delay()`只在`LCD.C`中被调用；
  
- 硬件的接口函数的命名规则`硬件名(大写)_函数名`,提供提供接口，在`_func.c`中进行声明，如`LCD_clear()`表示LCD屏幕的清空，在`LCD_func.h`中声明

## 实现思路
- 硬件代码和逻辑代码独立，硬件代码编译完后向外提供接口函数

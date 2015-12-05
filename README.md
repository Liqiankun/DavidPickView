DavidPickerView
=============================
EASIER to use UIDatePicker and UIDataPicker. When I wanna find a pickeView with a toolBar, I got ZHPickView. ZHPickView is the best one that I can find! But it isn't good enough! It still has some issues. So I decided to fix them.DavidPickerView is based on [ZHPickView](http://code4app.com/ios/ZHPickView/54783f73933bf09c1d8b46ed "悬停显示"). 

How To Use
=========================
Drag DavidPickerView to your project. Then `import "DavidPickerView.h"`.<br>
Like this:<br>
```c
//initWithPlistFile
-(instancetype)initPickviewWithPlistName:(NSString *)plistName isHaveNavControler:(BOOL)isHaveNavControler;

//initWithArray
-(instancetype)initPickviewWithArray:(NSArray *)array isHaveNavControler:(BOOL)isHaveNavControler withTitle:(NSString*)titleStr;

//initDatePickView
-(instancetype)initDatePickWithDate:(NSDate *)defaulDate datePickerMode:(UIDatePickerMode)datePickerMode isHaveNavControler:(BOOL)isHaveNavControler withTitle:(NSString*)titleStr;
```

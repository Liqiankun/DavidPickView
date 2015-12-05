DavidPickView
=============================
EASIER to use UIDatePicker and UIDataPicker. When I wanna find a pickeView with a toolBar, I got ZHPickView. ZHPickView is the best one that I can find! But it isn't good enough! It still has some issues. So I decided to fix them.DavidPickView is based on [ZHPickView](http://code4app.com/ios/ZHPickView/54783f73933bf09c1d8b46ed "悬停显示"). 

How To Use
=========================
Drag DavidPickView to your project. Then `import "DavidPickerView.h"`.<br>
Like this:<br>
```c
//initWithPlistFile
-(instancetype)initPickviewWithPlistName:(NSString *)plistName isHaveNavControler:(BOOL)isHaveNavControler;

//initWithArray
-(instancetype)initPickviewWithArray:(NSArray *)array isHaveNavControler:(BOOL)isHaveNavControler withTitle:(NSString*)titleStr;

//initDatePickView
-(instancetype)initDatePickWithDate:(NSDate *)defaulDate datePickerMode:(UIDatePickerMode)datePickerMode isHaveNavControler:(BOOL)isHaveNavControler withTitle:(NSString*)titleStr;

/**
 *   remove pickView from superView
 */
-(void)remove;
/**
 *  show pickView at currentView
 */
-(void)show;
/**
 *  set pickView background color
 */
-(void)setPickViewColer:(UIColor *)color;
/**
 *  set toolbar TinColor
 */
-(void)setTintColor:(UIColor *)color;
/**
 *  set toolbar background color
 */
-(void)setToolbarTintColor:(UIColor *)color;
```

Delegate
===========

```c
/**
 *  @param pickVeiw  The pickView         
 *  @param resultString Result of pickView
 */
-(void)toobarDonBtnHaveClick:(DavidPickView *)pickView resultString:(NSString *)resultString;
```
Call when click at confirmation button.
```c
/**
 *  @param pickVeiw  The pickView         
 */
-(void)didClickCancelItem:(DavidPickView *)pickView;
```
Call when click at cancel button

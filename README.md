# DropDownMenuList

dropList 选择控件   
自适应弹出方向、支持搜索  
  
use:    
DropDownMenuList * upDropMenu = [[DropDownMenuList alloc] init];  
NSMutableArray * titleAry;  
CGRect btnFrame = [self.view convertRect:_upChoseView.frame toView:self.view];  
//upDropMenu.isCanMatchStr = YES/NO;  
[upDropMenu showDropDownMenu:btnFrame arrayOfTitle:titleAry];  
upDropMenu.clickIndex = ^(long cindex) {  
     vc.upChoseText.text = [titleAry objectAtIndex:cindex];  
};  
[self.view addSubview:upDropMenu];    

![](https://github.com/aaa510665117/DropDownMenuList/raw/master/dropMenuListGif.gif)  

# DropDownMenuList

dropList 选择控件   
自适应位置、支持搜索  
  
use:    
DropDownMenuList * upDropMenu = [[DropDownMenuList alloc] init];  
NSMutableArray * titleAry = [[NSMutableArray alloc]init];  
CGRect btnFrame = [self.view convertRect:_upChoseView.frame toView:self.view];  
upDropMenu.isCanMatchStr = YES/NO;  
[upDropMenu showDropDownMenu:btnFrame arrayOfTitle:titleAry];  
pDropMenu.clickIndex = ^(long cindex) {  
     vc.upChoseText.text = [titleAry objectAtIndex:cindex];  
};  
[self.view addSubview:upDropMenu];    

![](https://github.com/aaa510665117/DropDownMenuList/raw/master/dropMenuListGif.gif)  

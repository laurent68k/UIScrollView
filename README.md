# UIScrollView
UIScrollView with Xcode 11: Content Layout Guides

Xcode 11: Issue with UIScrollView
     
     https://stackoverflow.com/questions/56570660/how-to-fix-scrollable-content-size-ambiguity-in-xcode-11-ios-12-ios-13-usin
     
     
First way:
     
     Disabling the content layout guides in properties
     
Second way:
     
     https://useyourloaf.com/blog/scroll-view-layouts-with-interface-builder/

Basically what you need is 9 constraints (assuming you want to scroll only vertically):

1-4: ScrollView to Superview (top, bottom, leading, trailing). Make sure to connect it to parent view and not to safe area.

5-8: Content view to Content Layout guide (top, bottom, leading, trailing).

     Content view Width equals width to Frame Layout Guide.
     

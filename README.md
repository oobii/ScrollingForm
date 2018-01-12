# ScrollingForm
ScrollingForm

When a stack view doesn't have a defined width or height, its size is based on its subviews. 
As you add content to the stack view, it expands to fit all your content. Thus the content inside the stack view defines 
the stack views size. It's only as big as it needs to be. Because stack views grow to fit their content, they are a perfect 
candidate for holding the content of a scroll view. As the content grows, the scroll view will scroll to meet the needs of 
the content size.

Observation: Here is the sequence that seems to work to create whats needed. First we add ScrollView which fill the whole parent view,then we add a dummmy view with Label and TextView sub views (with Auto Layout configured for them), and only then we add StackView to be the parent view of the dummy view. Then we “Control-drag from this dummy view to the view controller's view and release. In the popover, choose Equal Widths.









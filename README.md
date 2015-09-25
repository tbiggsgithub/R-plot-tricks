# R-plot-tricks

Superscripts in axis text:  
```R
x=seq(1:5)
y=seq(2:6)
xlab= expression(paste("4"^"th"))
plot(x,y,xlab=xlab)
```

Superscripts in axis labels for plots with several panels (subplots):
```R
		mtext(expression(paste("Irrig area, 000km"^"2")),side=2,line=2)
```

Axis label with embedded subscripts (above examples allow subscript at the end of the string but not return to regular script (here, on y-axis):
```R
  plot(x,y,ylab="")
  mtext(expression('z'['0m']*' m'),side=2,line=2)
```

Make axes flush with intersection:  in plot line, set xaxs=”i”

Rotate y-axis labels to horizontal:  in plot line, set las=1
	
No boundary box:  frame.plot=FALSE

+ 负边距margin
        <div id="container">
          <div id="center"></div>
        </div>
        <div id="left"></div>
        <div id="right"></div>

  把中间的模块center用container包裹起来，container设置width: 100%; float: left; center<br/>
  模块： left right container( center ) float: left;<br/>
  container width:100%;占据整个上部； float: left;<br/>
  center: margin-left: x px; margin-right: a px; 中间的模块 设置左右边距 给left,right模块让出空间；<br/>
  left: width: a px; margin-left: -100%; left模块原本在下部的紧贴左边的边,负边距-100%，向左移100%浏览器界面宽度左贴住，所以向上再左移；<br/>
  right: width: b px; margin-left: right-width px; 原理同left;<br/>

+ position:
  left center right Html中位置无关<br/>
  center正常文档流中；设置左右margin，给left,right模块让出空间；<br/>
  left,right模块position: absolute; 脱离文档流；top: 0; <br/>
  left模块 设置宽度， left: 0;<br/>
  right模块：设置宽度， right: 0;<br/>
  当中间有内部有固定宽度的元素或设有最小宽度，缩小时 会发生重叠


+ float:
       <div id="left"></div>
       <div id="right"></div>
       <div id="center"></div>

  left: float: left; width: ~px; 脱离文档流<br/>
  right: float: right; width: ~px; 脱离文档流<br/>
  center: margin左右边距; 正常文档流<br/>
  right得在center前，不然center的右边距挡住right;<br/>

+ 关键：边距， 脱离文档流
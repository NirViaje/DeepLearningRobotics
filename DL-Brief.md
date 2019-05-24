# DL in an hour, a personal perspective

![](img/nurbs-data-manifold.png)

## Fundament

1. Fit, aprroximation, interpolation, estimation, predict

<!-- ![](img/GaussFitExample_3.png) -->
![](img/Curve-Fitting-Toolbox.jpg)

2. case in real life, spline
    * https://www.ibiblio.org/e-notes/Splines/nurbs.html
    * https://www.ibiblio.org/e-notes/Splines/bezier3d.html

![](img/Bezier-patch.png)

2. Universal [approximation](https://zhuanlan.zhihu.com/p/23186434) theorem
    * [UAT](https://en.wikipedia.org/wiki/Universal_approximation_theorem)
    
    ![](img/UAT.png)
    
    * spline appr
    
    ![](img/headus-poly-to-nurbs-car.jpg)
    <!-- <canvas id="canvas" width="500" height="500"></canvas>  -->

    * multi-diemensions

    ![](img/Photography_cheat_sheet_digital_processing.jpg)

    * image, cases of low dimension embedded

    ![](img/stanford_statues_manifold.jpg)
    ![](img/manifold-face.png)

4. https://github.com/NirViaje/DeepLearningRobotics/blob/master/NeuronTalk.md
    * Hebbian, naive ANN
      * where the neuron is?
      
      ![](img/Hebbian.png)

      * matrix and non-linear
      
      ![](img/single-artificial-neuron.png)
      ![](img/Feed-forward-neural-network-with-sigmoid-activation-function-X-i-i-1P-input.png)
      ![](img/real-valued-binary-networks.png)

    * XOR, [multi-layer](https://playground.tensorflow.org/)

    ![](img/playground-tensorflow-single-layer.png)
    ![](img/playground-tensorflow-2-hidden.png)

    * principle


      * info redundant, constrain (cnn, dimension reduction

    ![](img/nurbs-data-manifold.png)

      * info distill (auto-encoder/LeNet

    ![](img/pixelspaceLinear.jpeg)
    
    * localize, convolution, primary visual cortex of mammal, DCT

      ![](img/DNN.jpg)

      * huge number of weights/paras

      ![](img/face-patches.png)
      
      * visual cortex, DCT

      ![](img/cconvdemo.png)
      ![](img/convolution-img-calc.png)
      ![](img/sparse-matrix-mul.jpg)
      ![](img/sparse-matrix-mul-vectors.png)

      * localize, convolution
    * LeNet, AlexNet, VGG, GoogLeNet inception, ResNet

    ![](img/CNN-anatomy.png)
    ![](img/simple-introduction-to-autoencoder-26-638.jpg)

      * timeline, go deep, [Autoencoder](https://www.slideshare.net/billlangjun/simple-introduction-to-autoencoder), Hinton 2006

    ![](img/cnn-1998-LeNet.jpg)

      0. LeNet, 1998

    ![](img/cnn-2012-alexnet-features.png)
    ![](img/cnn-2012-alexnet.png)
    ![](img/cnn-2012-alexnet-calc.png)

      1. [AlexNet](https://my.oschina.net/u/876354/blog/1633143), 2012,  ImageNet Challenge

    ![](img/cnn-2014-A-visualization-of-the-VGG-architecture.png)

      2. [Vgg](https://blog.csdn.net/qq_40027052/article/details/79015827), 2014, Visual Geometry Group - University of Oxford

    ![](img/cnn-2014-GoogLeNet-anatomy.png)
    ![](img/cnn-2014-GoogLeNet-arch.jpg)

      3. [GoogLeNet inception](https://my.oschina.net/u/876354/blog/1637819), 2014

    ![](img/cnn-1998-LeNet.jpg)

      4. ResNet, 2015 Dec

    ![](img/cnn-2015-resnet-layer.jpg)
    ![](img/cnn-2015-resnet-bottleneck-layer.jpg)

      * [Survey](https://www.topbots.com/a-brief-history-of-neural-network-architectures/)

    ![](img/nnarch13_eNet.png)
    ![](img/nnarch-calc.png)
    ![](img/cnn-evolve.png)
    ![](img/cnn-survey-go-deeper.jpg)


      * build blocks, [ReLu 1996/2010](https://www.zhihu.com/question/61265076/answer/260492479), with leakage, pooling, dropout etc

    ![](img/relu-common-nonlinear-activation-functions.png)
    ![](img/ReLu-adv.jpg)

      * optimization, training, backpropagation, [Andrew Ng's course](https://mooc.study.163.com/smartSpec/detail/1001319001.htm)

      ![](img/bp-output_1_backprop-4.png)
      ![](img/bp-nn-calculation.png)

5. Gu@SUNY, manifold

    ![](img/manifold-Gu-640.webp)

6. what's more
    * detect, track, Yolo/openPose etc
    * LSTM
    * GAN
    * DRL
    
    ![image](https://user-images.githubusercontent.com/1320252/58313710-cb942080-7e40-11e9-855c-e8132e852b4a.png)
    ![](img/openai-robotics.png)
    ![](img/intell-stages.jpg)
    * connect concrete and abstract
      * [Deep Learning and Geometry, by Xianfeng Gu](https://mp.weixin.qq.com/s/Upkci9ovvrlmA7EhqmNd0g)
      * the figure of three stage
    * further methodology
      * non-BP
      * unsupervised
      * etc
7. a little bit more on AGI
    * [AIXI](https://www.zhihu.com/question/34393952/answer/65205814)
    * ![](https://pic1.zhimg.com/80/c88b9731c98a2271b744347856f6706c_hd.png)
8. fully DL rendered movie?
    * [nVidia be a render company again](https://zhuanlan.zhihu.com/p/31627466)
 
## HandsOn

1. available workbench in lab
    * 1080Tix3
    * P40x2
2. [Deepo](https://github.com/ufoym/deepo)
3. [git](http://www.ruanyifeng.com/blog/2015/12/git-cheat-sheet.html)

## Several Cases

1. on Aesthetic, eyes movement
2. [scratch2code](https://zhuanlan.zhihu.com/p/33277230)
3. [coloring](https://zhuanlan.zhihu.com/p/31965450)
4. more


<!-- <script src="https://www.ibiblio.org/e-notes/Splines/CanvasMatrix.js" type="text/javascript"></script>

<script id="shader-vs" type="x-shader/x-vertex"> 
  attribute vec3 aPos;
  attribute vec3 aNorm;
  uniform mat4 mvMatrix;
  varying vec4 color;
  const vec4 dirDif = vec4(0., 0., -1., 0.);
  const vec4 dirHalf = vec4(-.4034, .259, .8776, 0.);
void main(void) {
   vec4 pos = mvMatrix * vec4(aPos, 1.);
   pos.z  = -.1*pos.z;
   gl_Position = pos;
   vec4 rotNorm = mvMatrix * vec4(aNorm, .0);
   float i = max( 0., abs(dot(rotNorm, dirDif)) );
   color = vec4(.0, .5*i, i, 1.);
   i = pow( max( 0., abs(dot(rotNorm, dirHalf)) ), 120.);
   color += vec4(i, i, i, 0.);
}
</script> 
 
<script id="shader-fs" type="x-shader/x-fragment"> 
precision mediump float;
  varying vec4 color;
void main(void) {
   gl_FragColor = color;
}
</script> 
 
<script id="line-vs" type="x-shader/x-vertex"> 
  attribute vec3 aPos;
  uniform mat4 mvMatrix;
void main(void) {
   gl_PointSize = 7.;
   vec4 pos = mvMatrix * vec4(aPos, 1.);
   pos.z  = -.1*pos.z;
   gl_Position = pos;
}
</script> 
 
<script id="line-fs" type="x-shader/x-fragment"> 
precision mediump float;
  uniform vec4 pCol;
void main(void) {
   gl_FragColor = pCol;
}
</script> 

<script type="text/javascript"> 
var p = new Float32Array(48);
var gl, canvas,  pi180 = 180/Math.PI, w, h, pointId = 0,
  transl, rTouch, fiTouch, idTouch0,
  xRot = yRot = zRot =  xOffs = yOffs =  drag = 0;
function startTouch(evt) {
  var evList = evt.touches;
  if(radio == "mesh"){
    if(evList.length == 1){
      xOffs = evList[0].pageX;  yOffs = evList[0].pageY;
      drag = 1;}
    else if(evList.length == 2){
      idTouch0 = evList[0].identifier;
      var dx = evList[1].pageX - evList[0].pageX;
      var dy = evList[1].pageY - evList[0].pageY;
      rTouch = Math.sqrt(dx*dx + dy*dy);
      fiTouch = Math.atan2(dy, dx);
      drag = 2;}
  }else{
    if(evList.length == 1){
      xOffs = evList[0].pageX;  yOffs = evList[0].pageY;
      pointId = getPointId(evt);
      drag = 1;}
  }
  evt.preventDefault();
}
function continueTouch(evt) {
  if ( drag == 0 ) return;
  if(radio == "mesh"){
    if(drag == 1){
      var x = evt.touches[0].pageX,  y = evt.touches[0].pageY;
      yRot = x - xOffs;  xRot = y - yOffs;
      xOffs = x;  yOffs = y;}
    else if(drag == 2){
      var dx = evt.touches[1].pageX - evt.touches[0].pageX;
      var dy = evt.touches[1].pageY - evt.touches[0].pageY;
      var r = Math.sqrt(dx*dx + dy*dy);
      var fi;
      if( idTouch0 == evt.touches[0].identifier ) fi = Math.atan2(dy, dx);
      else fi = Math.atan2(-dy, -dx);
      transl *= rTouch / r;
      zRot = pi180*(fiTouch - fi);
      rTouch = r;  fiTouch = fi;
    }
  }else if(drag == 1){
    var x = evt.touches[0].pageX - xOffs,  y = -(evt.touches[0].pageY - yOffs);
    p[pointId] += (rotMat.m11*x + rotMat.m12*y)*2*transl/w;
    p[pointId + 1] += (rotMat.m21*x + rotMat.m22*y)*2*transl/w;
    p[pointId + 2] += (rotMat.m31*x + rotMat.m32*y)*2*transl/w;
    bezier();
    xOffs = evt.touches[0].pageX;  yOffs = evt.touches[0].pageY;
  }
  drawScene();
}
function stopTouch() {
  drag = 0;
}
function mymousedown( ev ){
  drag  = 1;
  xOffs = ev.clientX;  yOffs = ev.clientY;
  if(radio == "point") pointId = getPointId(ev);
}
function getPointId(ev){
   var c = getXY(ev);
   var Rmin = 2,  Id = 0;
   for (var i = 0; i < 48; i += 3){
    var x = (rotMat.m11*p[i] + rotMat.m21*p[i+1] + rotMat.m31*p[i+2])/transl - c[0];
    var y = (rotMat.m12*p[i] + rotMat.m22*p[i+1] + rotMat.m32*p[i+2])/transl - c[1];
    var r2 = x*x + y*y;
    if ( r2 < Rmin ){ Id = i; Rmin = r2;}}
   return Id;
}
function getXY(ev){
  if (!ev.clientX) ev = ev.touches[0];
  var rect = canvas.getBoundingClientRect();
  var x = 2*(ev.clientX - rect.left)/w - 1,
      y = 2*(h - (ev.clientY - rect.top))/h - 1;
  return [x, y];
}
function mymousemove( ev ){
  if ( drag == 0 ) return;
  var x = ev.clientX - xOffs,  y = -(ev.clientY - yOffs);
  if(radio == "mesh"){
    if ( ev.shiftKey ) {
      transl *= 1 - y/1000;
      zRot = -x*.3; }
    else {
      yRot =  x;  xRot = -y; }
  } else{
    p[pointId] += (rotMat.m11*x + rotMat.m12*y)*2*transl/w;
    p[pointId + 1] += (rotMat.m21*x + rotMat.m22*y)*2*transl/w;
    p[pointId + 2] += (rotMat.m31*x + rotMat.m32*y)*2*transl/w;
    bezier();
  }
  xOffs = ev.clientX;   yOffs = ev.clientY;
  drawScene();
}
function wheelHandler(ev) {
  var del = 1.1;
  if (ev.shiftKey) del = 1.01;
  var ds = ((ev.detail || ev.wheelDelta) > 0) ? del : (1 / del);
  transl *= ds;
  drawScene();
  ev.preventDefault();
}
function getShader ( gl, id ){
   var shaderScript = document.getElementById ( id );
   var str = "";
   var k = shaderScript.firstChild;
   while ( k ){
     if ( k.nodeType == 3 ) str += k.textContent;
     k = k.nextSibling;
   }
   var shader;
   if ( shaderScript.type == "x-shader/x-fragment" )
           shader = gl.createShader ( gl.FRAGMENT_SHADER );
   else if ( shaderScript.type == "x-shader/x-vertex" )
           shader = gl.createShader(gl.VERTEX_SHADER);
   else return null;
   gl.shaderSource(shader, str);
   gl.compileShader(shader);
   if (gl.getShaderParameter(shader, gl.COMPILE_STATUS) == 0)
      alert(id + "\n" + gl.getShaderInfoLog(shader));
   return shader;
}
function initGL(){
   canvas = document.getElementById("canvas");
   if (!window.WebGLRenderingContext){
     alert("Your browser does not support WebGL. See http://get.webgl.org");
     return;}
   try { gl = canvas.getContext("experimental-webgl");
   } catch(e) {}
   if ( !gl ) {alert("Can't get WebGL"); return;}
   canvas.addEventListener('DOMMouseScroll', wheelHandler, false);
   canvas.addEventListener('mousewheel', wheelHandler, false);
   canvas.addEventListener('mousedown', mymousedown, false);
   canvas.addEventListener('mouseup', stopTouch, false);
   canvas.addEventListener('mousemove', mymousemove, false);
   canvas.addEventListener('touchstart', startTouch, false);
   canvas.addEventListener('touchmove', continueTouch, false);
   canvas.addEventListener('touchend', stopTouch, false);
}

var prog, line_prog, bonds = true, mvMatLine, mvMatLoc, pColLoc;
var mvMatrix = new CanvasMatrix4();
var rotMat = new CanvasMatrix4();
var n = 100, n1 = n+1, radio = "mesh";
function webGLStart() {
   transl = 3;
   initGL();
   var size = Math.min(window.innerWidth, window.innerHeight) - 10;
   canvas.width =  size;   canvas.height = size;
   w = h = size;
   gl.viewport(0, 0, size, size);

   prog  = gl.createProgram();
   gl.attachShader(prog, getShader( gl, "shader-vs" ));
   gl.attachShader(prog, getShader( gl, "shader-fs" ));
   posLoc = 0;
   gl.bindAttribLocation(prog, posLoc, "aPos");
   normLoc = 1;
   gl.bindAttribLocation(prog, normLoc, "aNorm");
   gl.linkProgram(prog);

   var k = 0;
   for (var j= 0; j< 4; j++) for (var i= 0; i< 4; i++){
     p[k++] = (i - 1.5);     p[k++] = (j -1.5);     p[k++] = -.0;}
   p[20] = p[17] = p[32] = p[29] = 2;
   bP = gl.createBuffer();
   bPoint = gl.createBuffer();
   bNorm = gl.createBuffer();

   var ind = [];
   for (var i = 0; i < n; i++ )
     for (var j = 0; j < n; j++ ){
       ind.push (i*n1+j); ind.push ((i+1)*n1+j+1); ind.push (i*n1+j+1);
       ind.push (i*n1+j); ind.push ((i+1)*n1+j); ind.push ((i+1)*n1+j+1);
     }
   ind.push(0,1,2,3, 4,5,6,7, 8,9,10,11, 12,13,14,15,
            0,4,8,12, 1,5,9,13, 2,6,10,14, 3,7,11,15);
   gl.bindBuffer(gl.ELEMENT_ARRAY_BUFFER, gl.createBuffer());
   gl.bufferData(gl.ELEMENT_ARRAY_BUFFER, new Uint16Array(ind),
     gl.STATIC_DRAW);

   line_prog  = gl.createProgram();
   gl.attachShader(line_prog, getShader( gl, "line-vs" ));
   gl.attachShader(line_prog, getShader( gl, "line-fs" ));
   lineLoc = 2;
   gl.bindAttribLocation(line_prog, lineLoc, "aPos");
   gl.linkProgram(line_prog);

   bezier();
   gl.enableVertexAttribArray( posLoc );
   gl.enableVertexAttribArray( normLoc );
   gl.enableVertexAttribArray( lineLoc );

   rotMat.makeIdentity();
   rotMat.rotate(-50,  1,0,0);
   mvMatLoc = gl.getUniformLocation(prog,"mvMatrix");
   mvMatLine = gl.getUniformLocation(line_prog,"mvMatrix");
   pColLoc = gl.getUniformLocation(line_prog,"pCol");

   gl.enable(gl.DEPTH_TEST);
   gl.clearDepth(100.0);
   gl.clearColor(0, 0, 0, 1);
   output = document.getElementById("output");

   drawScene();

  canvas.resize = function (){
    var size = Math.min(window.innerWidth, window.innerHeight) - 10;
    canvas.width =  size;   canvas.height = size;
    w = h = size;
    gl.viewport(0, 0, size, size);
    drawScene();
  }
}
function bezier(){
   var st = 1/n;
   var b0 = new Float32Array(n1), b1 = new Float32Array(n1),
       b2 = new Float32Array(n1), b3 = new Float32Array(n1),
       d0 = new Float32Array(n1), d1 = new Float32Array(n1),
       d2 = new Float32Array(n1), d3 = new Float32Array(n1);
   for (var i = 0; i <= n; i++){
      var u = i*st, u1 = 1-u, u12 = u1*u1, u2 = u*u,
      db0 = 3*u12, db3 = 3*u2,  t = 5*u*u1;
      b0[i] = u1*u12; b1[i] = db0*u; b2[i] = db3*u1; b3[i] = u*u2;
      d0[i] = -db0; d1[i] = db0 - t; d2[i] = t - db3; d3[i] = db3;
   }
   var pt = new Float32Array(3*n1*n1),  nt = new Float32Array(3*n1*n1);
   var k = 0;
   for (var j= 0; j< n1; j++) for (var i= 0; i< n1; i++){
    var x1 = (
     (p[0]*b0[i]  + p[3]*b1[i]  + p[6]*b2[i]  + p[9]*b3[i])*d0[j] +
     (p[12]*b0[i] + p[15]*b1[i] + p[18]*b2[i] + p[21]*b3[i])*d1[j] +
     (p[24]*b0[i] + p[27]*b1[i] + p[30]*b2[i] + p[33]*b3[i])*d2[j] +
     (p[36]*b0[i] + p[39]*b1[i] + p[42]*b2[i] + p[45]*b3[i])*d3[j] );
    var y1 = (
     (p[1]*b0[i]  + p[4]*b1[i]  + p[7]*b2[i]  + p[10]*b3[i])*d0[j] +
     (p[13]*b0[i] + p[16]*b1[i] + p[19]*b2[i] + p[22]*b3[i])*d1[j] +
     (p[25]*b0[i] + p[28]*b1[i] + p[31]*b2[i] + p[34]*b3[i])*d2[j] +
     (p[37]*b0[i] + p[40]*b1[i] + p[43]*b2[i] + p[46]*b3[i])*d3[j] );
    var z1 = (
     (p[2]*b0[i]  + p[5]*b1[i]  + p[8]*b2[i]  + p[11]*b3[i])*d0[j] +
     (p[14]*b0[i] + p[17]*b1[i] + p[20]*b2[i] + p[23]*b3[i])*d1[j] +
     (p[26]*b0[i] + p[29]*b1[i] + p[32]*b2[i] + p[35]*b3[i])*d2[j] +
     (p[38]*b0[i] + p[41]*b1[i] + p[44]*b2[i] + p[47]*b3[i])*d3[j] );
    var x2 = (
     (p[0]*d0[i]  + p[3]*d1[i]  + p[6]*d2[i]  + p[9]*d3[i])*b0[j] +
     (p[12]*d0[i] + p[15]*d1[i] + p[18]*d2[i] + p[21]*d3[i])*b1[j] +
     (p[24]*d0[i] + p[27]*d1[i] + p[30]*d2[i] + p[33]*d3[i])*b2[j] +
     (p[36]*d0[i] + p[39]*d1[i] + p[42]*d2[i] + p[45]*d3[i])*b3[j] );
    var y2 = (
     (p[1]*d0[i]  + p[4]*d1[i]  + p[7]*d2[i]  + p[10]*d3[i])*b0[j] +
     (p[13]*d0[i] + p[16]*d1[i] + p[19]*d2[i] + p[22]*d3[i])*b1[j] +
     (p[25]*d0[i] + p[28]*d1[i] + p[31]*d2[i] + p[34]*d3[i])*b2[j] +
     (p[37]*d0[i] + p[40]*d1[i] + p[43]*d2[i] + p[46]*d3[i])*b3[j] );
    var z2 = (
     (p[2]*d0[i]  + p[5]*d1[i]  + p[8]*d2[i]  + p[11]*d3[i])*b0[j] +
     (p[14]*d0[i] + p[17]*d1[i] + p[20]*d2[i] + p[23]*d3[i])*b1[j] +
     (p[26]*d0[i] + p[29]*d1[i] + p[32]*d2[i] + p[35]*d3[i])*b2[j] +
     (p[38]*d0[i] + p[41]*d1[i] + p[44]*d2[i] + p[47]*d3[i])*b3[j] );
    var x3 = y1*z2 - y2*z1,  y3 = x2*z1 - x1*z2,  z3 = x1*y2 - x2*y1;
    var norm = Math.sqrt(x3*x3 + y3*y3 + z3*z3);
    nt[k] = x3/norm;
    pt[k++] = (
     (p[0]*b0[i]  + p[3]*b1[i]  + p[6]*b2[i]  + p[9]*b3[i])*b0[j] +
     (p[12]*b0[i] + p[15]*b1[i] + p[18]*b2[i] + p[21]*b3[i])*b1[j] +
     (p[24]*b0[i] + p[27]*b1[i] + p[30]*b2[i] + p[33]*b3[i])*b2[j] +
     (p[36]*b0[i] + p[39]*b1[i] + p[42]*b2[i] + p[45]*b3[i])*b3[j] );
    nt[k] = y3/norm;
    pt[k++] = (
     (p[1]*b0[i]  + p[4]*b1[i]  + p[7]*b2[i]  + p[10]*b3[i])*b0[j] +
     (p[13]*b0[i] + p[16]*b1[i] + p[19]*b2[i] + p[22]*b3[i])*b1[j] +
     (p[25]*b0[i] + p[28]*b1[i] + p[31]*b2[i] + p[34]*b3[i])*b2[j] +
     (p[37]*b0[i] + p[40]*b1[i] + p[43]*b2[i] + p[46]*b3[i])*b3[j] );
    nt[k] = z3/norm;
    pt[k++] = (
     (p[2]*b0[i]  + p[5]*b1[i]  + p[8]*b2[i]  + p[11]*b3[i])*b0[j] +
     (p[14]*b0[i] + p[17]*b1[i] + p[20]*b2[i] + p[23]*b3[i])*b1[j] +
     (p[26]*b0[i] + p[29]*b1[i] + p[32]*b2[i] + p[35]*b3[i])*b2[j] +
     (p[38]*b0[i] + p[41]*b1[i] + p[44]*b2[i] + p[47]*b3[i])*b3[j] );
   }
   gl.bindBuffer(gl.ARRAY_BUFFER, bPoint);
   gl.bufferData(gl.ARRAY_BUFFER, pt, gl.STATIC_DRAW);
   gl.vertexAttribPointer(posLoc, 3, gl.FLOAT, false, 0, 0);

   gl.bindBuffer(gl.ARRAY_BUFFER, bNorm);
   gl.bufferData(gl.ARRAY_BUFFER, nt, gl.STATIC_DRAW);
   gl.vertexAttribPointer(normLoc, 3, gl.FLOAT, false, 0, 0);

   gl.bindBuffer(gl.ARRAY_BUFFER, bP);
   gl.bufferData(gl.ARRAY_BUFFER, p, gl.STATIC_DRAW);
   gl.vertexAttribPointer(lineLoc, 3, gl.FLOAT, false, 0, 0);
}
function setN(v) {
  n = parseInt(v);  n1 = n + 1;
  webGLStart();
}
function drawScene(){
  rotMat.rotate(xRot/3, 1,0,0);  rotMat.rotate(yRot/3, 0,1,0);
  rotMat.rotate(zRot, 0,0,1);
  yRot = xRot = zRot = 0;
  rotMat.m44 = transl;
  gl.clear(gl.COLOR_BUFFER_BIT | gl.DEPTH_BUFFER_BIT);
  gl.useProgram(prog);
  gl.uniformMatrix4fv( mvMatLoc, false, new Float32Array(rotMat.getAsArray()) );
  gl.drawElements(gl.TRIANGLES, 6*n*n, gl.UNSIGNED_SHORT, 0);
  if (bonds){
    gl.useProgram(line_prog);
    gl.uniformMatrix4fv( mvMatLine, false, new Float32Array(rotMat.getAsArray()) );
    gl.uniform4f( pColLoc, 1, 1, 1, 1 );
    gl.drawArrays(gl.POINTS, 0, 16);
    for (var i = 0; i < 8; i++ )
      gl.drawElements(gl.LINE_STRIP, 4, gl.UNSIGNED_SHORT, 12*n*n + i*8);
  }
  var x = rotMat.m11*p[0] + rotMat.m21*p[1] + rotMat.m31*p[2]; 
  var y = rotMat.m12*p[0] + rotMat.m22*p[1] + rotMat.m32*p[2]; 
  output.innerHTML = " x= " + round(x) +" y= "+ round(y);
}
function round(v){ return Math.round(1000*v/transl)/1000; }
</script>  -->

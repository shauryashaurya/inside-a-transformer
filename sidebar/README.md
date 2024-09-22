# issues and remedies    
Things I run into and resolve while developing this project    
     
1. Numpy 2.x breaks backwards compatibility. Modules like pandas, plotly and others will have to migrate to Numpy 2.x    
	* [Release Notes](https://numpy.org/doc/stable/release/2.0.0-notes.html)    
	* [NumPy 2.0 migration guide](https://numpy.org/doc/stable/numpy_2_0_migration_guide.html#numpy-2-migration-guide)  
	
2. Onnx on windows is breaking.   
	* Error: ```DLL load failed while importing onnx_cpp2py_export: A dynamic link library (DLL) initialization routine failed.```    
	* [On GitHub](https://github.com/onnx/onnx/issues/6267), [another](https://github.com/Gourieff/comfyui-reactor-node/issues/384)   
	* following [this solution first](https://github.com/onnx/onnx/issues/6267#issuecomment-2356072424), was on ``` onnx 1.16.2```, downgraded to ```onnx 1.16.1```, works   
	* wasted almost 1 hour of my life.   
	* heard the phrase **"the boons and banes of open source"** - not a good thing for open source. *We can do better.*  
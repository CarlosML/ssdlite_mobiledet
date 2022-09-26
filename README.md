# ssdlite_mobiledet
Output of converting ssdlite_mobiledet_cpu_320x320_coco_2020_05_19 with OpenVINO 2022.2.0 with 

mo.py
--framework=tf --data_type=FP32 
--output_dir=. --model_name=ssdlite_mobiledet
--reverse_input_channels
'--input_shape=[1,320,320,3]'
--tensorflow_object_detection_api_pipeline_config=./ssdlite_mobiledet_cpu_320x320_coco_2020_05_19/pipeline.config
--input_model=./ssdlite_mobiledet_cpu_320x320_coco_2020_05_19/tflite_graph.pb
--output raw_outputs/box_encodings,convert_scores

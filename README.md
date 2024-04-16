I tried to finetune YOLOv8 on TPU VM v4-8 but I failed

Why I failed?
YOLOv8 backbone on keras cv use broadcast layer and it's not supported by TPU / XLA compilation. Perhaps I can construct a custom class that have static layer size to adapt with training data, but maybe another time LOL.

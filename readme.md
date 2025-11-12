# TR-LLM: Integrating Trajectory Data for Scene-Aware LLM-Based Human Action Prediction

We present a multi-modal human action prediction framework that incorporates both an LLM and human trajectories. The core idea is to integrate two different perspectives—physical and semantic factors—through an object-based action prediction framework to reduce uncertainties and enhance action prediction accuracy. This github repo provides codes and evaluation data to test our model.

[Project website](https://sites.google.com/view/tr-llm/%E3%83%9B%E3%83%BC%E3%83%A0)

[arxiv paper](https://arxiv.org/abs/2410.03993)

<div align="center">
<img src="./Overview.jpg" width="600" height="800" />
</div>

## Quick start
Quick visualization of the trajectories contained in LocoVR is done by the following instructions.

1. Download github repo

3. Download model
Download the foloder "model_path_gen" and "model_goal_pred" from [this link](https://drive.google.com/drive/folders/1D1ogzcJUhUx6zpITXC15zI7MVbgEWfz7?usp=sharing), and unzip it, then place it in the top of "main" folder.
     
4. Install the packages in requirements.txt (python==3.8.1, cuda12.1):
```
pip install -r requirements.txt
```
5. Set API key and Organization code 
   Open setting.py in the main folder, and replace "*******" at API_KEY with your original information.
   
6. Calculate
   Run TR-LLM.py, then it will generate results in "Result" folder.
```
python ./main/TR-LLM.py
```

7. Evaluate
   Run Evaluation.sh to get quantitative and qualitative evaluation results.
```
bash ./main/eval.py
```  

## Citation
If you find this repo useful for your research, please consider citing:

@inproceedings{takeyama2025trllm,
  title        = {TR-LLM: Integrating Trajectory Data for Scene-Aware LLM-Based Human Action Prediction},
  author       = {Takeyama, Kojiro and Liu, Yimeng and Sra, Misha},
  booktitle    = {Proceedings of the IEEE/RSJ International Conference on Intelligent Robots and Systems (IROS)},
  year         = {2025},
  month        = {October},
  address      = {Hangzhou, China},
  publisher    = {IEEE},
  organization = {IEEE/RSJ},
  note         = {Accepted to IROS 2025; also available as arXiv:2410.03993}
}


## License
This project is licensed under the MIT License

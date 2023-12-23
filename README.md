# SW-tips
In this file I write the steps I have followed to install or uninstall some softwares either on my mac or linux os:
-----------------------------------------------------------------------------------------------------------------
#How to deal with GPU in linux
If you want to use GPU in your deep learning project you may need to use GPU, and for this mean you need to install graphic driver in my case it is nvidia.
I found this link very useful. [https://www.cyberciti.biz/faq/ubuntu-linux-install-nvidia-driver-latest-proprietary-driver/]
## I downloaded GPU driver on linux for using it in my project with following way:
- Open apps and software and select the one at the top which is specified by a pranthesis (test, ...)
- You need to reboot system. It is possible both with the terminal via `sudo reboot` or you can restart your laptop.
- After installing GPU drives you can verify it using this command: `nvidia-smi`
- then I used this command ro install CUDA toolkit: `sudo apt-get install nvidia-cuda-toolkit`
- After installing GPU drives you can verify it using this command: `nvcc --version`
- However, if you've made changes and want to start with a clean slate before following the provided instructions, you can uninstall the GPU   drivers, CUDA Toolkit, cuDNN, and any deep learning frameworks you've installed. Here's a step-by-step guide:  
```
sudo apt-get purge nvidia*
sudo apt-get autoremove
sudo apt-get autoclean
```
  --------------------------------------------------------------------------------------------------------------

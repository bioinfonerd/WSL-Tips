# Windows SubSystem Tips

# Installing Docker
https://nickjanetakis.com/blog/setting-up-docker-for-windows-and-wsl-to-work-flawlessly

# Installing Jupyter Notebook

You can run the jupyter notebook from anywhere (i.e., from the Linux or Windows filesystem). The WSL will act as a jupyter server accessible at localhost with port 8888.

Install jupyter: pip3 install jupyter
Create alias to launch jupyter without browser from the WSL: 
- Open your bash configuration: vim ~/.bashrc
- Add to the end of the file and save/exit:
alias jupyter-notebook="~/.local/bin/jupyter-notebook --no-browser"
- Update your bash profile: source ~/.bashrc
Now you can run a jupyter server jupyter-notebook and access the service with your browser from Windowslocalhost:8888.

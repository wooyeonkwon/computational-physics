# Special topics in deep learning for big data

## Use a password-protected SSH key
### prerequisite
* should have github account 
* add ssh-key to your github account following the [instrouction](https://docs.github.com/en/github/authenticating-to-github/generating-a-new-ssh-key-and-adding-it-to-the-ssh-agent)

Here is the quick summary.

```
ssh yourid@IP-address
ssh-keygen -t ed25519 -C "your_email@example.com"
cat ~/.ssh/id_ed25519.pub
```
copy the line of the outcome and paste it to [add the SSH key to the github acccount](https://docs.github.com/en/github/authenticating-to-github/adding-a-new-ssh-key-to-your-github-account).

Just login to the dedicated machine and type following lines. 

```
ssh yourid@IP-address
git clone git@github.com:monttj/computational-physics.git
cd computational-physics
./jupyter.sh 
```

And follow the instruction. That's it! 


## Alternative using the web URL

Just login to the dedicated machine and type following lines.

```
ssh yourid@IP-address
git clone https://github.com/monttj/computational-physics.git
cd computational-physics
./jupyter.sh 
```

And follow the instruction. That's it! 

## Environment setup

You need to install anaconda. In your conda environment, need to install tensorflow, Keras, notebook, ipykernel. 
This can be done with following scripts. 

If you have already downloaded git repository, update it so that the scripts can be checked out. 
```
cd computational-physics
git pull 
```

Then run following scripts. This is only one time setup. 
```
./Miniconda2-latest-Linux-x86_64.sh
./setup.sh
```

Finally, run the jupyter
```
./jupyter.sh 
```





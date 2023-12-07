# mysamples

CC0 sample bank
## Adding samples to Estuary using !reslist

To add these samples into Estuary type the following in the Terminal Window and press Enter:
```
!reslist "https://djmelan3.github.io/mysamples/resources.json" 
```

## Preparing Audio Samples

See https://github.com/cleary/Clean-Samples#advice-for-preparing-samples on some advice on how to prepare audio samples. Also ensure that each sample is placed in it's own folder. If multiple files of the same sample exist (for example, in the case that the sample has been pitch-shifted and separate files exist of each pitch-shifted sample) make sure all these are in the same folder. To see what the file structure looks like, simply refer back to this repository (e.g. bassb).

## Instructions for Contributing to this repository

Important: Please ensure that all samples you contribute are samples where you are 100% sure that either (a) you are the original creator and thus copyright holder, or (b) the samples are are clearly and verifiably in the public domain. Consider adding a .txt file to any folder you add briefly indicating how the samples were produced.

- Create an account on github.com (just once).

- Fork the repository by going to the central copy of it on github at https://github.com/djmelan3/mysamples.git and clicking on the
Fork button (just once).

- Using a command shell, clone *your*copy* of the repository from github to a computer in your possession. For example:

```
cd~
git clone https://github.com/djmelan3/mysamples.git
````

- Add sample folders and files to the "mysamples" folder on your computer (if you follow the instruction above exactly,
it will be in your home folder).

- To share changes with others, first check what differences exist in your folder:

```
cd ~/mysamples
git status
````

- If the list of changed files from git status looks right, add them all to a pending commit (terminal code here assumes
you are still in the "mysamples" folder):

```
git add .
```

- By contrast, *if* the list isn't completely right, you can get around this by adding the right things one by one:

```
git add someSampleFolder/someSoundFile.wav
```

- After you've added, wrap that up as a "commit" with a descriptive message and push it to your github.com copy of the repository:

```
git commit -m "a message describing what you are changing/adding"
git push
```

- Go on github.com, to the page about your copy of the repository, and click pull request.

- To get an updated version of the central copy from time to time, you must first have added + committed any of your own
changes, then:

```
cd ~/mysamples
git pull https://github.com/djmelan3/mysamples.git main
```

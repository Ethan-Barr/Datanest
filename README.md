# DataNexus

DataNexus is a simple to use Python module that you can use in your projects to get transcripts, datasets, etc.
The module also allows you to extract character lines from transcripts witch makes it easyer for you to be able to do finetunning of a GPT2 model as an example.

## Key feactures
- Downloading of Datasets and Transcripts
- Extract Characters from Transcripts


## Installation
To get started:
```
pip install datanexus
```



## Usage

⚠️ | Full documenation link to come in the future and the code may be unstable as in testing!

### Downloading of Datasets/Transcripts
```py
from datanexus import datanexus

datanexus = datanexus()

datasets = datanexus.download_dataset('ironman.txt')
print(datasets)
```


### Extract character's from transcripts
You will need to create a folder called `Models` to sucessfully extract the character information
```py
from datanexus import datanexus

character = datanexus.save_character('ironman.txt', 'Tony Stark:', 'Tony.txt')
print(character)
```
## Showing all of the possible datasets
This function will show all of the possible datasets that is usable
```py
from datanexus import datanexus

datasets = datanexus.possible_models()

for dataset in datasets:
    print(dataset)
```


## Support
If you have any question or any issues then feel free to create an issue on [Github](https://github.com/Ethan-Barr/DataNexus). 

Feel free to join [The Workshop](https://discord.gg/sm2ZdxvU6y) discord server and send me a ping (`_Ethan_`)
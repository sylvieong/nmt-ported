To run the code in Pycharm:
- File -> New Project (point to nmt-ported)
- In Pycharm, right-click on nmt-ported folder -> Mark Directory as -> Sources Root
- Do the same with nmt folder
- Set command line parameters as "Script parameters" in Run/Debug Configurations. Example:i
Script: /home/song/projects/nmt-ported/nmt/nmt.py
Script parameters: --src=vi --tgt=en  --vocab_prefix=/home/song/tmp/nmt_data/vocab   --train_prefix=/home/song/tmp/nmt_data/train  --dev_prefix=/home/song/tmp/nmt_data/tst2012   --test_prefix=/home/song/tmp/nmt_data/tst2013  --out_dir=/home/song/tmp/nmt_model  --num_train_steps=12000  --steps_per_stats=100  --num_layers=2  --num_units=128  --dropout=0.2 --metrics=bleu

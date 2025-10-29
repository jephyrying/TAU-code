
- Download the TextZoom dataset from: https://github.com/JasonBoy1/TextZoom.
- Download the pre-trained recognizers from:
  - ASTER: https://github.com/ayumiymk/aster.pytorch.
  - CRNN: https://github.com/meijieru/crnn.pytorch.
  - MORAN: https://github.com/Canjie-Luo/MORAN_v2.
  - PARSeq: https://github.com/baudm/parseq.
  
# train
  python main.py --batch_size="48" --mask --rec="aster" --srb="1" --pre_training

# test
  python main.py --batch_size="48" --mask --rec="aster" --srb="1" --resume="./ckpt/checkpoint.pth" --pre_training --test --test_data_dir="/root/dataset/TextZoom/test/easy"

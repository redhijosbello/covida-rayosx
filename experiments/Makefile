chest-xray-pneumonia.zip:
	kaggle datasets download paultimothymooney/chest-xray-pneumonia

data/chest-xray:
	mkdir -p data/raw
	unzip chest-xray-pneumonia.zip -d data/raw

chest-xray-dataset: \
	chest-xray-pneumonia.zip \
	data/chest-xray
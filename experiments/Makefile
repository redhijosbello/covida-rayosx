chest-xray-pneumonia.zip:
	kaggle datasets download paultimothymooney/chest-xray-pneumonia

data/chest-xray:
	mkdir -p data
	unzip chest-xray-pneumonia.zip -d data/

chest-xray-dataset: \
	chest-xray-pneumonia.zip \
	data/chest-xray
chest-xray-pneumonia.zip:
	kaggle datasets download paultimothymooney/chest-xray-pneumonia

data/chest-xray:
	mkdir -p data/raw
	unzip chest-xray-pneumonia.zip -d data/raw

clear_dataset_chest_xray:
	rm -r data/raw/chest_xray/__MACOSX
	rm -r data/raw/chest-xray/chest-xray

get_chest_xray_dataset: \
	chest-xray-pneumonia.zip \
	data/chest-xray \
	clear_dataset_chest_xray
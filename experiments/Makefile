chest-xray-pneumonia.zip:
	kaggle datasets download paultimothymooney/chest-xray-pneumonia

data/raw/chest_xray:
	mkdir -p data/raw
	unzip chest-xray-pneumonia.zip -d data/raw
	rm -r data/raw/chest_xray/__MACOSX # eliminamos datos innecesarios
	rm -r data/raw/chest_xray/chest_xray # ídem

get_chest_xray_dataset: \
	chest-xray-pneumonia.zip \
	data/raw/chest_xray 
#################### Dataset de Kaggle de neumonía ####################

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

#################### Dataset de covid ####################

covid-xray.zip:
	wget https://github.com/ieee8023/covid-chestxray-dataset/archive/master.zip
	mv master.zip covid-xray.zip

data/raw/covid_xray:
	mkdir -p data/raw
	unzip covid-xray.zip -d data/raw
	mv data/raw/covid-chestxray-dataset-master data/raw/covid_xray

get_covid_xray_dataset: \
	covid-xray.zip \
	data/raw/covid_xray
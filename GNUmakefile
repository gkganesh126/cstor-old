# Specify the date o build
BUILD_DATE = $(shell date +'%Y%m%d%H%M%S')

cstor-main-image: 
	@echo "----------------------------"
	@echo pwd
	@echo "--> cstor-main-image         "
	@echo "----------------------------"
	@sudo docker build -f Dockerfile.maincontainer -t openebs/cstor:ci --build-arg BUILD_DATE=${BUILD_DATE} .	
	@sh push

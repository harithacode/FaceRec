# FaceRec
A simple java web application to id faces in images using the faceplusplus API 

Faceplusplus API is an face recognition API that is available for free limited usage. This application assumes that persons and groups were created and the faceplusplus server has been trained with faces of those persons.

(for more information visit: http://www.faceplusplus.com/)

This application has been tested in jetty.(Class files not included in the repository)

It takes a single type of request which is an image url and sends the url to faceplusplus server for recognition. Then it receives the results from faceplusplus server and constructs a toned down version of those results in json. This was for a class project and the toned down version of json was more convenient for the collaborating teams than the original json response of the faceplusplus server.

Note: The faceplusplus API key and key secret are hardcoded in Line 38 of FaceRecognition.java in onsap package. The group name to compare the picture against is hardcoded in line 41 of the same file. (like: serverParams.setGroupName("cricketers");) 



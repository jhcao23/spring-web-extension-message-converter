Simply create MappingStringJackson2HttpMessageConverter which extends AbstractJackson2HttpMessageConverter 
<= as typical MappingJackson2HttpMessageConverter is not sufficient for wechat official account API 
<- but this is due to wechat server sometimes sends wrong MediaType in response header. 

`mvn clean install deploy -DperformRelease=true`

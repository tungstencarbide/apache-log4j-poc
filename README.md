# Apache-Log4j
Apache Log4j 远程代码执行

> 攻击者可直接构造恶意请求，触发远程代码执行漏洞。漏洞利用无需特殊配置，经阿里云安全团队验证，Apache Struts2、Apache Solr、Apache Druid、Apache Flink等均受影响

![image](https://user-images.githubusercontent.com/45926593/145425339-47c71230-87d2-4519-8919-9c3520850f83.png)


### 修复方案：

（1）修改jvm参数
-Dlog4j2.formatMsgNoLookups=true

（2）修改配置
在应用classpath下添加log4j2.component.properties配置文件，log4j2.formatMsgNoLookups=true

Bad English Translation:
# Apache-Log4j
Apache Log4j remote code execution

Attackers can directly construct malicious requests to trigger remote code execution vulnerabilities. No special configuration is required for exploiting vulnerabilities.
The security team verified that Apache Struts2, Apache Solr, Apache Druid, Apache Flink, etc. are all affected

![image](https://user-images.githubusercontent.com/45926593/145425339-47c71230-87d2-4519-8919-9c3520850f83.png)


### Mitigation plan:

(1) Modify jvm parameters
-Dlog4j2.formatMsgNoLookups=true

(2) Modify the configuration
Add the log4j2.component.properties configuration file under the application classpath, log4j2.formatMsgNoLookups=true
~

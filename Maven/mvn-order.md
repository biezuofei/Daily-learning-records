# maven -- order line

 Give it a try.

	Maven�������
	
	Maven�⣺
	
	http://repo.maven.org/maven2/
	
	Maven������ѯ��
	
	http://mvnrepository.com/
	һ��Maven�������
	
	1. ����Maven����ͨJava��Ŀ��
	
	mvn archetype:create
	    -DgroupId=packageName
	    -DartifactId=projectName
	
	2. ����Maven��Web��Ŀ��
	
	mvn archetype:create
	    -DgroupId=packageName
	    -DartifactId=webappName
	    -DarchetypeArtifactId=maven-archetype-webapp
	
	3. �������� maven ��Ŀ�ĹǼܣ�
	
	mvn archetype:generate
	
	����������ô�������maven��Ŀ��?�ǲ���������:
	
	mvn archetype:create -DarchetypeArtifactId=maven-archetype-quickstart -DgroupId=com.ryanote -Dartifact=common
	
	��������㻹���õĻ�,�����out��,�ִ��˶���mvn archetype:generate��,����������Ŀ���������¸������Ի�,����Ҳ����Ҫ����ô���archetypeArtifactId,��ֻ������archetype:generate,ʣ�µľ�������ѡ���⡱��.
	
	����cmd���裺
	
	������дд����
	
	mvn archetype:generate -DgroupId=otowa.user.dao -DartifactId=user-dao -Dversion=0.01-SNAPSHOT
	
	4. ����Դ���룺
	
	mvn compile
	
	5. ������Դ��룺
	
	mvn test-compile
	
	6. ���в���:
	
	mvn test
	
	7. ����site��
	
	mvn site
	
	8. �����
	
	mvn package
	
	9. �ڱ���Repository�а�װjar��
	
	mvn install
	����installing D:\xxx\xx.jar to D:\xx\xxxx
	
	10. �����������Ŀ��
	
	mvn clean
	
	11. ����eclipse��Ŀ��
	
	mvn eclipse:eclipse
	
	12. ����idea��Ŀ��
	
	mvn idea:idea
	
	13. ���ʹ��goal�����ֻ��������ԣ�
	
	mvn -Dtest package
	
	14. ������Ե����ݣ�
	
	mvn test-compile
	
	15. ֻ��jar��:
	
	mvn jar:jar
	
	16. ֻ���Զ������룬Ҳ�����Ա��룺
	
	mvn test -skipping compile -skipping test-compile
	 ( -skipping ��������ã���ȻҲ�������������������) 
	
	17. ���eclipse��һЩϵͳ����:
	
	mvn eclipse:clean 
	
	18.�鿴��ǰ��Ŀ�ѱ�������������
	
	mvn dependency:list
	
	19.�ϴ���˽����
	
	mvn deploy
	
	20. ǿ�Ƽ����£����ڿ��հ汾�ĸ��²���(һ����¼��Ρ�����ʱ�����һ��)���ڣ������ǿ�Ƹ��¾ͻ��õ�������: 
	
	mvn clean install-U
	
	21. Դ������
	
	mvn source:jar
	��
	mvn source:jar-no-fork
	
	mvn compile��mvn install��mvn deploy������
	
	    mvn compile���������ļ�
	    mvn install������mvn compile��mvn package��Ȼ���ϴ������زֿ�
	    mvn deploy,����mvn install,Ȼ���ϴ���˽��
	
	����PS:
	
	����һ��ʹ�����������������ͨ��cvs��svn���ش��뵽������Ȼ��ִ��mvn eclipse:eclipse����ecllipse��Ŀ�ļ���Ȼ���뵽eclipse�����ˣ��޸Ĵ����ִ��mvn compile��mvn test���飬Ҳ��������eclipse��maven�����
	
	1. ��ʾ�汾��Ϣ :
	
	mvn -version/-v
	
	2. ����mvn��Ŀ:
	
	mvn archetype:create -DgroupId=com.oreilly -DartifactId=my-app
	
	3. ����targetĿ¼�����롢���Դ��룬���ɲ��Ա��棬����jar/war�ļ� :
	
	mvn package
	
	4. ������Ŀ��jetty��:
	
	mvn jetty:run
	
	5. ��ʾ��ϸ���� ��Ϣ:
	
	mvn -e
	
	6. ��֤�����Ƿ���ȷ��������Ҫ����Դ�Ƿ����:
	
	mvn validate
	
	7. �ڼ��ɲ��Կ������еĻ����д���ͷ�����:
	
	mvn integration-test
	
	8. �����κμ�飬��֤���Ƿ���Ч�Ҵﵽ������׼:
	
	mvn verify
	
	9. ����Ӧ����Ҫ���κζ����Դ���룬��xdoclet :
	
	mvn generate-sources
	
	10. ʹ�� help �����  describe Ŀ������� Maven Help �������Ϣ:
	
	mvn help:describe -Dplugin=help
	
	11. ʹ��Help �����������Ĵ��в�����Ŀ���� :
	
	mvn help:describe -Dplugin=help -Dfull
	
	12. ��ȡ����Ŀ�����Ϣ,����  mojo ������  plugin �������������г���Compiler �����compile Ŀ���������Ϣ :
	
	mvn help:describe -Dplugin=compiler -Dmojo=compile -Dfull
	
	13. �г����� Maven Exec ������õ�Ŀ��:
	
	mvn help:describe -Dplugin=exec -Dfull
	
	14. ���������Ч�� (effective)��POM������¶�� Maven��Ĭ������ :
	
	mvn help:effective-pom
	
	15. ��Ҫ�鿴�����������ټ���������Щ��Ϊ��ͻ��������ԭ������ܾ�����Ĺ������� Maven �ĵ��Ա������ :
	
	mvn install -X
	
	16. ���κ�Ŀ�����maven.test.skip ���Ծ����������� :
	
	mvn install -Dmaven.test.skip=true
	
	17. ����װ��Maven Assembly �����һ������������Ӧ�ó������зַ����Ĳ�� :
	
	mvn install assembly:assembly
	
	18. ����Wtp�����Web��Ŀ :
	
	mvn -Dwtpversion=1.0 eclipse:eclipse
	
	19. ���Eclipse��Ŀ��������Ϣ(Web��Ŀ) :
	
	mvn -Dwtpversion=1.0 eclipse:clean
	
	20. ����Ŀת��ΪEclipse��Ŀ :
	
	mvn eclipse:eclipse
	
	21. mvn exec�������ִ����Ŀ�е�main���� :
	
	������Ҫ����java���̣�mvn compile
	�����ڲ���������£�mvn exec:java -Dexec.mainClass="***.Main"
	���ڲ�����mvn exec:java -Dexec.mainClass="***.Main" -Dexec.args="arg0 arg1 arg2"
	ָ������ʱ�⣺mvn exec:java -Dexec.mainClass="***.Main" -Dexec.classpathScope=runtime
	
	22. ��ӡ���ѽ���������б� :
	
	mvn dependency:resolve
	
	23. ��ӡ���������� :
	
	mvn dependency:tree
	
	��Ӧ�ó�����ʹ�ö���洢�� 
	���ƴ���
	
	<repositories>    
	    <repository>     
	        <id>Ibiblio</id>     
	        <name>Ibiblio</name>     
	        <url>http://www.ibiblio.org/maven/</url>   
	    </repository>   
	    <repository>     
	        <id>PlanetMirror</id>     
	        <name>Planet Mirror</name>     
	        <url>http://public.planetmirror.com/pub/maven/</url>   
	    </repository>  
	</repositories>
	
	mvn deploy:deploy-file -DgroupId=com -DartifactId=client -Dversion=0.1.0 -Dpackaging=jar -Dfile=d:\client-0.1.0.jar -DrepositoryId=maven-repository-inner -Durl=ftp://xxxxxxx/opt/maven/repository/
	
	���ƴ���
	����������Jar�����ؿ���
	���ƴ���
	
	mvn install:install-file -DgroupId=com -DartifactId=client -Dversion=0.1.0 -Dpackaging=jar -Dfile=d:\client-0.1.0.jar
	
	
	-DdownloadSources=true
	
	-DdownloadJavadocs=true
	
	���ƴ���
	��������
	
	mvn help:describe
	
	���Ƿ���Ϊ�ǲ���ĳ���������Щgoal��ʹ���,���Ƿ���Ϊ�벻��ĳ��goal����Щ����������,�Ǿ�������������,���������һ�е�.
	
	����: 1. -Dplugin=pluginName   2. -Dgoal(��-Dmojo)=goalName:��-Dpluginһ��ʹ��,�����г�ĳ�������goal��Ϣ,
	
	����Ӳ�����ϸ,ͬ�����Լ�-Ddetail.(ע:һ�����goalҲ����Ϊ��һ�� ��Mojo��)
	
	�����Ҿ�����mvn help:describe -Dplugin=help -Dmojo=describe����һ�°�!
	
	mvn tomcat:run
	
	����maven��,����Ҳ����Ҫ��eclipse���tomcat������web��Ŀ(ʵ�ʹ����о����ᷢ����������ֲ�ͬ�����µ����),ֻ���ڶ�ӦĿ¼������ mvn tomat:run����,Ȼ��Ϳ�������������в鿴��.�������Ҫ����Ķ���,������pom.xml�ļ������������:
	
	01 02 03 04 org.codehaus.mojo 05 tomcat-maven-plugin 06 07 /web 08 9090 09 10 11 12 ��Ȼ��Ҳ������������Ӳ�����ʵ���ض��Ĺ���,
	
	���漸���Ƚϳ���:
	
	����1>. ��������:-Dmaven.test.skip(=true)
	
	����2>. ָ���˿�:-Dmaven.tomcat.port=9090
	
	����3>. ���Բ���ʧ��:-Dmaven.test.failure.ignore=true ��Ȼ,����������������Ŀ�й����µĻ�,һ��Ҫ����Ŀ��Ŀ¼������mvn clean install��ִ�и���,������mvn tomcat:runʹ�Ķ���Ч.
	
	mvnDebug tomcat:run
	
	����������Ҫ����Զ�̲���,�������Զ�̲����õ�8000�˿�,��eclipse���Զ�̲��Ժ�,���ͻ���������,��ϵ�,����,һ�ж�����ô��.�����ᵽ���Ǽ�������������ͬ������.
	
	mvn dependency:sources
	
	����˼��,������,��Ͳ��õ�����Դ����,����һ��,����Ŀ����������jar����Դ��Ͷ�����

```bash
$ vim --bar
```

See `man mvn` for more details.

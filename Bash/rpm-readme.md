Redhat linux bash rpm 
===

#һ��rpm RPM���������;��
	1�����԰�װ��ɾ���������͹����������ȻҲ֧�����߰�װ�����������
	2��ͨ��RPM��������֪�������������Щ�ļ���Ҳ��֪��ϵͳ�е�ĳ���ļ������ĸ��������
	3�������ڲ�ѯϵͳ�е�������Ƿ�װ�Լ���汾��
	4����Ϊ�����߿��԰��Լ��ĳ�����ΪRPM ��������
	5�������ǩ��GPG��MD5�ĵ��롢��֤��ǩ������
	6�������Եļ�飬�鿴�Ƿ�����������ڲ����ݶ�������ϵͳ��
#����RPM ��ʹ��Ȩ�ޣ�
	RPM����İ�װ��ɾ��������ֻ��rootȨ�޲���ʹ�ã����ڲ�ѯ�����κ��û������Բ����������ͨ�û�ӵ�а�װĿ¼��Ȩ�ޣ�Ҳ���Խ��а�װ
#����rpm ��һ����÷�
	һ����ʼ��rpm ���ݿ⣻
	
	ͨ��rpm �����ѯһ��rpm ���Ƿ�װ�ˣ�Ҳ��Ҫͨ��rpm ���ݿ�����ɵģ���������Ҫ�����������������������ʼ��rpm ���ݿ⣻
	
	rpm --initdb
	rpm --rebuilddb ע�����Ҫ���ó�ʱ�䣻
	
	ע�������������Ǽ�Ϊ���ã���ʱrpm ϵͳ�������⣬���ܰ�װ�Ͳ�ѯ�����������������⣻
	����RPM���������Ĳ�ѯ���ܣ�
	1����ϵͳ���Ѱ�װ����Ĳ�ѯ��
	
	1����ѯϵͳ�Ѱ�װ�������
	�﷨��rpm -q �����
	
	������
	rpm -q gaim
	gaim-1.3.0-1.fc4
	
	-q���� --query ��������˼�ǡ��ʡ����������ʾ���ǣ��ǲ���ϵͳ��װ��gaim ������Ѱ�װ������Ϣ��������û�а�װ�������gaim û�а�װ����Ϣ��
	
	�鿴ϵͳ�������Ѿ���װ�İ���Ҫ�� -a ���� ��
	
	rpm -qa
	
	
	�����ҳ�鿴���ټ�һ���ܵ� |��more���
	
	rpm -qa |more
	
	�������Ѿ���װ��������в���ĳ�����������˵ gaim �������� grep ��ȡ������
	
	rpm -qa |grep gaim
	2����ѯһ���Ѿ���װ���ļ������ĸ��������
	
	�﷨ rpm -qf �ļ���
	
	
	ע���ļ������ڵľ���·��Ҫָ��
	
	������
	
	rpm -qf /usr/lib/libacl.la
	libacl-devel-2.2.23-8
	
	3����ѯ�Ѱ�װ���������װ���δ���
	
	�﷨��rpm -ql ����� �� rpm rpmquery -ql �����
	
	������
	
	rpm -ql lynx
	rpmquery -ql lynx
	
	4����ѯһ���Ѱ�װ���������Ϣ
	
	�﷨��ʽ�� rpm -qi �����
	
	������
	
	rpm -qi lynx
	
	5���鿴һ���Ѱ�װ����������ļ���
	
	�﷨��ʽ��rpm -qc �����
	
	������
	
	rpm -qc lynx
	
	6���鿴һ���Ѿ���װ������ĵ���װλ�ã�
	
	�﷨��ʽ�� rpm -qd �����
	
	������
	
	[root@localhost RPMS]# rpm -qd lynx
	
	7���鿴һ���Ѱ�װ�������������������ļ���
	
	�﷨��ʽ�� rpm -qR �����
	
	������
	
	rpm -qR rpm-python
	
	��ѯ�Ѱ�װ������ܽ᣺����һ��������Ѿ���װ�����ǿ��԰�һϵ�еĲ�����������ã����� rpm -qil �����磺
	
	rpm -qil lynx
	
	
	2������δ��װ��������Ĳ鿴��
	
	�鿴��ǰ��������һ��.rpm ���ļ���Ҳ����˵�Լ������file.rpm�Ĳ鿴�ȣ�
	
	1���鿴һ�����������;���汾����Ϣ��
	
	�﷨�� rpm -qpi file.rpm
	
	������
	
	rpm -qpi lynx-2.8.5-23.i386.rpm
	
	2���鿴һ����������������ļ���
	
	�﷨�� rpm -qpl file.rpm
	
	������
	
	rpm -qpl lynx-2.8.5-23.i386.rpm
	
	3���鿴��������ĵ����ڵ�λ�ã�
	
	�﷨�� rpm -qpd file.rpm
	
	������
	
	rpm -qpd lynx-2.8.5-23.i386.rpm
	
	5���鿴һ��������������ļ���
	
	�﷨�� rpm -qpc file.rpm
	
	������
	
	rpm -qpc lynx-2.8.5-23.i386.rpm
	
	4���鿴һ���������������ϵ
	
	�﷨�� rpm -qpR file.rpm
	
	������
	
	rpm -qpR yumex_0.42-3.0.fc4_noarch.rpm
	/bin/bash
	/usr/bin/python
	config(yumex) = 0.42-3.0.fc4
	pygtk2
	pygtk2-libglade
	rpmlib(CompressedFileNames) <= 3.0.4-1
	rpmlib(PayloadFilesHavePrefix) <= 4.0-1
	usermode
	yum >= 2.3.2
	����������İ�װ��������ɾ���ȣ�
	
	
	1����װ������һ��rpm ����
	
	[root@localhost beinan]#rpm -vih file.rpm ע�������������װһ���µ�rpm ����
	[root@localhost beinan]#rpm -Uvh file.rpm ע��������������һ��rpm ����
	
	�����������ϵ�ģ�����������ϵ����ʵ������������ܺܺõĽ��������ϵ���뿴ǰ���������������Ľ��ܣ���������������������Ҳ�Ҳ���������ϵ�İ�����ֻ��ͨ���������������İ������������ϵ������ǿ�ư�װ��
	
	�﷨�ṹ��
	
	rpm -ivh file.rpm --nodeps --force
	rpm -Uvh file.rpm --nodeps --force
	
	����Ĳ�������鿴 man rpm
	
	����Ӧ�ã�
	
	rpm -ivh lynx-2.8.5-23.i386.rpm
	Preparing... ########################################### [100%]
	   1:lynx ########################################### [100%]
	rpm -ivh --replacepkgs lynx-2.8.5-23.i386.rpm
	Preparing... ########################################### [100%]
	   1:lynx ########################################### [100%]
	
	ע�� --replacepkgs ���������Ѱ�װ������ٰ�װһ�Σ���ʱû��̫��ı�Ҫ��
	
	���԰�װ���� --test ���������������ϵ�������������İ�װ��
	
	rpm -ivh --test gaim-1.3.0-1.fc4.i386.rpm
	Preparing... ########################################### [100%]
	
	���°汾����Ϊ�ɰ汾��Ҫ�� --oldpackage ������
	
	rpm -qa gaim
	gaim-1.5.0-1.fc4
	rpm -Uvh --oldpackage gaim-1.3.0-1.fc4.i386.rpm
	Preparing... ########################################### [100%]
	   1:gaim ########################################### [100%]
	rpm -qa gaim
	gaim-1.3.0-1.fc4
	
	Ϊ�����ָ����װĿ¼��Ҫ�� -relocate ����������ľ����ǰ�gaim-1.3.0-1.fc4.i386.rpmָ����װ�� /opt/gaim Ŀ¼�У�
	
	rpm -ivh --relocate /=/opt/gaim gaim-1.3.0-1.fc4.i386.rpm
	Preparing... ########################################### [100%]
	   1:gaim ########################################### [100%]
	ls /opt/
	gaim
	
	Ϊ�����ָ����װĿ¼��Ҫ�� -relocate ����������ľ����ǰ�lynx-2.8.5-23.i386.rpm ָ����װ�� /opt/lynx Ŀ¼�У�
	
	
	rpm -ivh --relocate /=/opt/lynx --badreloc lynx-2.8.5-23.i386.rpm
	Preparing... ########################################### [100%]
	1:lynx ########################################### [100%]
	
	���ǰ�װ��ָ��Ŀ¼�еĳ�����ε����أ�һ��ִ�г��򣬶����ڰ�װĿ¼��bin����sbinĿ¼�У�����������ӣ�����д��������������Ӧ�����ӣ��� ln -s ��
	
	/opt/lynx/usr/bin/lynx
	Configuration file /etc/lynx.cfg is not available.
	ln -s /opt/lynx/etc/lynx.cfg /etc/lynx.cfg
	/opt/lynx/usr/bin/lynx www.linuxsir.org
	
	
	2��ɾ��һ��rpm ����
	
	������Ҫѧ���ѯrpm �� ���뿴ǰ���˵����
	
	rpm -e �������
	
	�����������Ƴ�lynx ���������Ĳ���Ӧ���ǣ�
	
	rpm -e lynx
	
	�����������ϵ����Ҳ������--nodeps ���������ļ����ɾ�����������ܲ�Ҫ��ô�������������������� systerm-config-packages ��ɾ��������������
	
	rpm -e lynx --nodeps
	
	
	�ġ�����ǩ����
	
	rpm --import ǩ���ļ�
	
	������
	
	rpm --import RPM-GPG-KEY
	rpm --import RPM-GPG-KEY-fedora
	
	����RPM��ǩ�����ܣ�������μ� man rpm
	
	�塢RPM�����������֧�����簲װ�Ͳ�ѯ��
	
	����������ͨ�� Fedora Core 4.0 ��һ�������ѯ����װ�������
	
	��ַ��
	http://mirrors.kernel.org/fedora/core/4/i386/os/Fedora/RPMS/
	
	������
	
	�����ʽ��
	
	rpm ���� rpm���ļ���http����ftp�ĵ�ַ
	
	# rpm -qpi http://mirrors.kernel.org/fedora/core/4/i386/os/ Fedora/RPMS/gaim-1.3.0-1.fc4.i386.rpm
	# rpm -ivh http://mirrors.kernel.org/fedora/core/4/i386/os/ Fedora/RPMS/gaim-1.3.0-1.fc4.i386.rpm
	
	��һ�����ɣ�
	
	
	�������Ѱ�װ�������ѯ��һ�㲹�䣻
	
	[root@localhost RPMS]# updatedb
	[root@localhost RPMS]# locate ��������ļ���
	
	ͨ��updatedb�����ǿ����� locate ����ѯһЩ�����װ�������ˣ�ϵͳ���ΰ�װʱҪִ��updatedb ��ÿ��һ��ʱ��ҲҪִ��һ�Σ��Ա����Ѱ�װ��������£�updatedb ��slocate��������У������û���������͵ð�װslocate ��
	
	������
	
	[root@localhost RPMS]# locate gaim
	
	
	
	�ߡ���rpm�������ȡ�ļ���
	
	�����ʽ�� rpm2cpio file.rpm |cpio -div
	
	
	������
	
	rpm2cpio gaim-1.3.0-1.fc4.i386.rpm |cpio -div
	
	��ȡ�������ļ����ڵ��ò���Ŀ¼�е� usr ��etc�У�
	
	��ʵ�����鵽�ļ�����ָ����װĿ¼����װ������ķ��㣻Ҳһ�����Գ���ļ���
	
	Ϊ�����ָ����װĿ¼��Ҫ�� -relocate ����������ľ����ǰ�gaim-1.3.0-1.fc4.i386.rpmָ����װ�� /opt/gaim Ŀ¼�У�
	
	rpm -ivh --relocate /=/opt/gaim gaim-1.3.0-1.fc4.i386.rpm
	Preparing... ########################################### [100%]
	   1:gaim ########################################### [100%]
	ls /opt/
	gaim
	
	����Ҳ��һĿ��Ȼ��gaim�������ļ����ǰ�װ�� /opt/gaim �У�����ֻ�ǰ�gaim Ŀ¼����һ�£�Ȼ��ж��gaim��������ʵҲ����ȡ�ļ���һ���÷���
	
	
	�ˡ�RPM�������ļ���
	
	RPM�������������ļ��� rpmrc �����ǿ������Լ���ϵͳ���ҵ�������Fedora Core 4.0�е�rpmrc �ļ�λ�ڣ�
	
	locate rpmrc
	/usr/lib/rpm/rpmrc
	/usr/lib/rpm/redhat/rpmrc
	
	���ǿ���ͨ�� rpm --showrc �鿴������Ļ��������Լ���ѧϰ���ǡ�������Ҫ���ң���Ҳ������ֻҪ��������ƪ���£���Ϊ�������ã�����ˮƽ�ͺ��Ҳ�ࣻ����ˮƽ��һ���ģ������Ҳ��ܰ������ˣ�����⣻
	
	src.rpm :
	ftp://ftp.redhat.com/pub/redhat/linux/enterprise/6Server/en/os/SRPMS/
	


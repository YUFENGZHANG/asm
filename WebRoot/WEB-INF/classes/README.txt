@title ��Ŀ˵��
@

1.������˵����
	......
	domain������ų־û�����model�ļ����൱����ʦ�Ͽν���model��
	vo��ֵ�������ڱ��治Ҫ�����ݿ����־û��Ķ�����ǰ̨��������ֵ�����Բ���vo��

2.beans.xml˵��
	beans.xml���Դﵽһ����Ŀ�����޸ģ�ʹ��ע��ķ�ʽ�򵥣���
	��1��ʹ��ע��ķ�ʽ������ע��
	<property name="packagesToScan">
			<list>
				<value>com.asm.domain</value>
			</list>
 	</property>
 	ʹ��domain���µ��������ܹ��Զ���ɨ���Ϊmodel,��ȥ����*.hbm,����Ҫ������������
 	@Entity
	@Table(name="t_employee")
	
	@Id
	@GeneratedValue(generator="employeeUUID")
	@GenericGenerator(name="employeeUUID", strategy="uuid")
	
	��2��action�н���ע�ⷽʽ������
	
	@SuppressWarnings("serial")
	@Controller("manageAction")
	@Scope("prototype")
	
	@Autowired
	
	��3��service �н���ע�ⷽʽ������
	����service����
	@Transactional(readOnly=true)
	@Service("employeeService")
	
	��4��dao�н���ע������
	@Repository("employeeDao")

3.jdbc.properties�������ݿ����ӵ�����
4.log4j.properties������־������
5.struts.xml
 	ÿ�����Լ������Լ���package����ʱ���Լ����ã�ͳһ���ɣ��Լ�ʹ���Լ�ϰ�ߵ����÷�ʽ
6.webroot��ֻ��һ��login.jsp�ļ�����������ת������ҳ�������WEB-INFĿ¼�£�һ��ģ��һ���ļ��У����ڴ�Ÿ�ģ��ҳ�棬��ֹ�Ƿ�����

	
 	
 	
# java1

 <bean id="transactionManager" class="org.springframework.orm.hibernate4.HibernateTransactionManager">
    <property name="sessionFactory" ref="sessionFactory" />
    </bean> 
    <tx:annotation-driven transaction-manager="transactionManager" />
    <tx:advice id="txAdvice" transaction-manager="transactionManager">
        <tx:attributes>

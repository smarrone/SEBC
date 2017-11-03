First line:

2017-11-03 05:02:26,420 INFO main:com.cloudera.server.cmf.Main: Starting SCM Server. JVM Args: [-Dlog4j.configuration=file:/etc/cloudera-scm-server/log4j.properties, -Dfile.encoding=UTF-8, -Dcmf.root.logger=INFO,LOGFILE, -Dcmf.log.dir=/var/log/cloudera-scm-server, -Dcmf.log.file=cloudera-scm-server.log, -Dcmf.jetty.threshhold=WARN, -Dcmf.schema.dir=/usr/share/cmf/schema, -Djava.awt.headless=true, -Djava.net.preferIPv4Stack=true, -Dpython.home=/usr/share/cmf/python, -XX:+UseConcMarkSweepGC, -XX:+UseParNewGC, -XX:+HeapDumpOnOutOfMemoryError, -Xmx2G, -XX:MaxPermSize=256m, -XX:+HeapDumpOnOutOfMemoryError, -XX:HeapDumpPath=/tmp, -XX:OnOutOfMemoryError=kill -9 %p], Args: [], Version: 5.11.2 (#6 built by jenkins on 20170811-0014 git: 3c3ea33a12076fb83a8f11c4452c52fac685d01b)




All lines containing the string "Started Jetty server"

2017-11-03 05:03:43,476 INFO WebServerImpl:org.springframework.web.servlet.handler.SimpleUrlHandlerMapping: Root mapping to handler of type [class org.springframework.web.servlet.mvc.ParameterizableViewController]
2017-11-03 05:03:43,580 INFO WebServerImpl:org.springframework.web.servlet.DispatcherServlet: FrameworkServlet 'Spring MVC Dispatcher Servlet': initialization completed in 5179 ms
2017-11-03 05:03:43,616 INFO WebServerImpl:com.cloudera.server.web.cmon.JobDetailGatekeeper: ActivityMonitor configured to allow job details for all jobs.
2017-11-03 05:03:45,348 INFO SearchRepositoryManager-0:com.cloudera.server.web.cmf.search.components.SearchRepositoryManager: Initializing SearchTemplateManager:2017-11-03T09:03:45.348Z
2017-11-03 05:03:45,392 INFO SearchRepositoryManager-0:com.cloudera.server.web.cmf.search.components.SearchRepositoryManager: Generating entities:2017-11-03T09:03:45.392Z
2017-11-03 05:03:45,407 INFO SearchRepositoryManager-0:com.cloudera.server.web.cmf.search.components.SearchRepositoryManager: Num entities:194
2017-11-03 05:03:45,407 INFO SearchRepositoryManager-0:com.cloudera.server.web.cmf.search.components.SearchRepositoryManager: Generating documents:2017-11-03T09:03:45.407Z
2017-11-03 05:03:45,879 INFO SearchRepositoryManager-0:com.cloudera.server.web.cmf.search.components.SearchRepositoryManager: Num docs:207
2017-11-03 05:03:45,881 INFO SearchRepositoryManager-0:com.cloudera.server.web.cmf.search.components.SearchRepositoryManager: Constructing repo:2017-11-03T09:03:45.881Z
2017-11-03 05:03:46,095 INFO WebServerImpl:com.cloudera.server.web.cmf.AggregatorController: AggregateSummaryScheduler started.
2017-11-03 05:03:46,756 INFO SearchRepositoryManager-0:com.cloudera.server.web.cmf.search.components.SearchRepositoryManager: Finished constructing repo:2017-11-03T09:03:46.756Z
2017-11-03 05:03:46,908 INFO WebServerImpl:org.mortbay.log: jetty-6.1.26.cloudera.4
2017-11-03 05:03:46,909 INFO WebServerImpl:org.mortbay.log: Started SelectChannelConnector@0.0.0.0:7180
2017-11-03 05:03:46,909 INFO WebServerImpl:com.cloudera.server.cmf.WebServerImpl: Started Jetty server.
2017-11-03 05:03:47,538 INFO ScmActive-0:com.cloudera.server.cmf.components.ScmActive: ScmActive completed successfully.

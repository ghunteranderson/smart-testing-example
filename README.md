Compare the results of `./mvnw test` and `./mvnw test -Dsmart.testing.disable=true`.
The second succeeds while the first results in this Surefire error.

```
[ERROR] Failed to execute goal org.apache.maven.plugins:maven-surefire-plugin:2.22.2:test (default-test) on project artifact: There are test failures.
[ERROR]
[ERROR] Please refer to C:\Users\HunterAnderson\github\tmp\smart-testing-example\target\surefire-reports for the individual test results.
[ERROR] Please refer to dump files (if any exist) [date].dump, [date]-jvmRun[N].dump and [date].dumpstream.
[ERROR] There was an error in the forked process
[ERROR] java.lang.IllegalStateException: No surefire provider implementation has been detected as applicable for your environment.
[ERROR] org.apache.maven.surefire.booter.SurefireBooterForkException: There was an error in the forked process
[ERROR] java.lang.IllegalStateException: No surefire provider implementation has been detected as applicable for your environment.
[ERROR]        at org.apache.maven.plugin.surefire.booterclient.ForkStarter.fork(ForkStarter.java:656)
[ERROR]        at org.apache.maven.plugin.surefire.booterclient.ForkStarter.run(ForkStarter.java:282)
[ERROR]        at org.apache.maven.plugin.surefire.booterclient.ForkStarter.run(ForkStarter.java:245)
[ERROR]        at org.apache.maven.plugin.surefire.AbstractSurefireMojo.executeProvider(AbstractSurefireMojo.java:1183)
[ERROR]        at org.apache.maven.plugin.surefire.AbstractSurefireMojo.executeAfterPreconditionsChecked(AbstractSurefireMojo.java:1011)
[ERROR]        at org.apache.maven.plugin.surefire.AbstractSurefireMojo.execute(AbstractSurefireMojo.java:857)
[ERROR]        at org.apache.maven.plugin.DefaultBuildPluginManager.executeMojo(DefaultBuildPluginManager.java:137)
[ERROR]        at org.apache.maven.lifecycle.internal.MojoExecutor.execute(MojoExecutor.java:210)
[ERROR]        at org.apache.maven.lifecycle.internal.MojoExecutor.execute(MojoExecutor.java:156)
[ERROR]        at org.apache.maven.lifecycle.internal.MojoExecutor.execute(MojoExecutor.java:148)
[ERROR]        at org.apache.maven.lifecycle.internal.LifecycleModuleBuilder.buildProject(LifecycleModuleBuilder.java:117)
[ERROR]        at org.apache.maven.lifecycle.internal.LifecycleModuleBuilder.buildProject(LifecycleModuleBuilder.java:81)
[ERROR]        at org.apache.maven.lifecycle.internal.builder.singlethreaded.SingleThreadedBuilder.build(SingleThreadedBuilder.java:56)
[ERROR]        at org.apache.maven.lifecycle.internal.LifecycleStarter.execute(LifecycleStarter.java:128)
[ERROR]        at org.apache.maven.DefaultMaven.doExecute(DefaultMaven.java:305)
[ERROR]        at org.apache.maven.DefaultMaven.doExecute(DefaultMaven.java:192)
[ERROR]        at org.apache.maven.DefaultMaven.execute(DefaultMaven.java:105)
[ERROR]        at org.apache.maven.cli.MavenCli.execute(MavenCli.java:957)
[ERROR]        at org.apache.maven.cli.MavenCli.doMain(MavenCli.java:289)
[ERROR]        at org.apache.maven.cli.MavenCli.main(MavenCli.java:193)
[ERROR]        at sun.reflect.NativeMethodAccessorImpl.invoke0(Native Method)
[ERROR]        at sun.reflect.NativeMethodAccessorImpl.invoke(NativeMethodAccessorImpl.java:62)
[ERROR]        at sun.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43)
[ERROR]        at java.lang.reflect.Method.invoke(Method.java:498)
[ERROR]        at org.codehaus.plexus.classworlds.launcher.Launcher.launchEnhanced(Launcher.java:282)
[ERROR]        at org.codehaus.plexus.classworlds.launcher.Launcher.launch(Launcher.java:225)
[ERROR]        at org.codehaus.plexus.classworlds.launcher.Launcher.mainWithExitCode(Launcher.java:406)
[ERROR]        at org.codehaus.plexus.classworlds.launcher.Launcher.main(Launcher.java:347)
[ERROR]        at sun.reflect.NativeMethodAccessorImpl.invoke0(Native Method)
[ERROR]        at sun.reflect.NativeMethodAccessorImpl.invoke(NativeMethodAccessorImpl.java:62)
[ERROR]        at sun.reflect.DelegatingMethodAccessorImpl.invoke(DelegatingMethodAccessorImpl.java:43)
[ERROR]        at java.lang.reflect.Method.invoke(Method.java:498)
[ERROR]        at org.apache.maven.wrapper.BootstrapMainStarter.start(BootstrapMainStarter.java:39)
[ERROR]        at org.apache.maven.wrapper.WrapperExecutor.execute(WrapperExecutor.java:122)
[ERROR]        at org.apache.maven.wrapper.MavenWrapperMain.main(MavenWrapperMain.java:61)
```

# Apache Tika OSGi bundle to work with [ForkParser](http://tika.apache.org/1.7/api/org/apache/tika/fork/ForkParser.html)
Use this bundle only when you need to use ForkParser in OSGi environment.
As ForkParser doesn't work with official bundle [tika-bundle](http://repo1.maven.org/maven2/org/apache/tika/tika-bundle/), so [DefaultParser](http://tika.apache.org/1.7/api/org/apache/tika/parser/DefaultParser.html) doesn't work with this bundle.

### Example usage in [Apache Karaf](http://karaf.apache.org/)
    <feature name="apache-tika" version="1.7">
        <bundle>mvn:org.apache.tika/tika-core/1.7</bundle>
        <bundle>mvn:org.apache.tika/tika-bundle-fork/1.7.2</bundle>
    </feature>

### Maven repository
There is no public maven repository with this bundle. You have to build and deploy it to your maven repository.

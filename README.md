This project for refactoring scr doc comment from declarative service file and and add those things to same file as osgi annotations.

Here

    Refactoring scr doc comment and convert it to OSGI annotations

    Replace the maven-scr-plugin from root pom dependency management

    If maven-scr-plugin is hard coded at the component pom then remove it

    Add the  org.apache.felix.scr.ds-annotations as dependency for each component pom if there has any declarative service

    Add the org.apache.felix.scr.ds-annotations as dependency for root pom

    Add the apache.felix.scr.ds.annotations.version(1.2.4) and  maven.scr.plugin.version(1.16.0) to parent pom properties.


User notes-

Here you should provide the repository names as command line argument. Repository name format should be like below example

example                                     

converter .sh wso2-extensions/identity-governance    wso2-extensions/identity-inbound-provisioning-scim2

You can view the final result from repo_result.txt (This file generated by the converter.sh)

Here final result will be categorized to three types. Those are

    Converted successful

    Converted unsuccessful

    Build failure 
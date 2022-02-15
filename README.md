**1. Pre-Destruction (destructiveChangesPre.xml):**

Consider a scenario where we need to delete components first and then update existing components or deploy new components. In this case, we can opt for the destructiveChangesPre.xml. In this process, the package will delete components first and then deploys existing components updates or new components. This means destructiveChangesPre.xml will execute first and then package.xml will be executed.

**2. Post-Destruction (destructiveChangesPost.xml):**

Consider a scenario where we need to update existing components or deploy new components first and then delete the components. In this case, we can opt for the destructiveChangesPost.xml. In this process, the package will deploy existing components updates or new components first and then delete the components. This means package.xml executes first and then destructiveChangesPost.xml will be executed.

**Naming convention for xml file**
If you are planning for PreDestructiveDeployment or PostDestructiveDeployment Or only Destructive then update file name destructivedepolymentpost.xml in above repository as be
PreDestructiveDeployment  => destructiveChangesPre.xml
PostDestructiveDeployment => destructiveChangesPost.xml
DestructiveDeployment     => destructiveChanges.xml


**Reference:**
1. https://www.v2force.com/blogs/destructive-deployment-with-metadata-api/

2. https://developer.salesforce.com/docs/atlas.en-us.daas.meta/daas/daas_destructive_changes.htm



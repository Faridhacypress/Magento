# Magento

1. clone this repo

2. open this directory in VS code

3. run command : npm install cypress

4. goto "node_modules\cypress-cucumber-preprocessor\lib\stepDefinitionPath.js"  file

   search for    :   confStepDefinitions || cypress${path.sep}integration;
   
   change to     :   confStepDefinitions || cypress${path.sep}e2e;


5. goto "node_modules\cypress-cucumber-preprocessor\lib\stepDefinitionPath.test.js"  file

   search for    :    const defaultNonGlobalStepDefinitionsPath = cypress${sep}integration;

   change to     :    const defaultNonGlobalStepDefinitionsPath = cypress${sep}e2e;

   
6. To  execute this script,

   run command : npx cypress open
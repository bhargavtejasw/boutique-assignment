ISSUE1-
imagepullbackoff for adcart service ,solved by changed v0.3.1 to v0.3.9
as v 0.3.1 is not present we upgraged the deployment with nearest version

ISSUE2-
crashbackoff error by cart service , solved by some kubectl logs analysis

ISSUE3 -
pending issue by redis-cart service solved it by removing the editing the deployment file ,removed node selector line from redis deployment as its not present 
then its started working 
 removed this -->Node-Selectors:   kubernetes.io/hostname=test-worker-2

ISSUE4-
again crashloopbackoff error by productcatalogservice ,solved by analysising kubectl  service logs


# Testing role 'jpnewman.json'

~~~
mkdir tmp

curl -XGET 'http://10.10.10.10:9200/.kibana/config/5.3.0?pretty=true' > kibana_config.json

ansible-playbook ./json.yml -i localhost.ini -c local -vvv
~~~

## Check Python

~~~
pep8 ../../library/json
~~~

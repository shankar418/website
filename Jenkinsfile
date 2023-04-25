pipeline
{
agent {label 'node1'}
stages
{
stage{'Build'}
{
steps
{
sh sudo docker rm -f $(sudo docker ps -a -q)
sh sudo docker build -it masterapp .
}
}

}
}

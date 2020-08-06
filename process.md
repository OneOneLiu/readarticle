前面的一切本地操作照旧

直到生成密钥这一步，输入命令ssh-keygen -t rsa -C "1183418633@qq.com"
生成后，连按三次回车即可，不要给密钥输入名字，然后去用户目录下检查发现密钥已经生成

随后，使用 git remote add origin git@github.com:OneOneLiu/readarticle.git先链接上目标的库

然后使用命令：git push -u origin master
，push即可

另外，如果目标库中已经有内容了，这时候需要先把它clone一份下来，然后cd到指定目录再进行修改

git clone git@github.com:OneOneLiu/readarticle.git 先把目标的库

最后要注意的一点是，修改了文件之后，好像都需要使用一次add命令，然后再commit才生效，不晓得是怎么回事，应该是我还没搞清楚
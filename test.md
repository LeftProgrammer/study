����Эͬ����
��Ϊ���¼������裺
1.����һ��git������� ��git init --bare��

2.������������汾���¡�����أ�git clone git�汾��������ַ��

3.���س������
git add �ļ���
git status 
git commit -m �ύ����������

4.���Ͱ汾�������� ��git remote +  git push origin master��
git remote	����֪�����������Ķ�
git push origin master	�������޸������ύ
5.��Զ�̷�������ȡ�汾��git pull��

��֧��ʹ��
��֧�Ļ�������
�������������¼�����

1. �鿴��ǰ��֧ ��git branch��

2. ������֧ ��git branch ��֧����

3.�л���֧��git checkout ��֧����

4.��֧�ϵĳ������
ʹ��git add ��git commit�ύ��
ʹ��git log�鿴����

5.��֧�ĺϲ� ��git checkout master + git merge ��֧����
git checkout master
git log
git merge ��֧��

6.��֧��ɾ����git branch -d ��֧����



you need to resolve your current index first ����취
��������Ҫ�Ƚ�����ǰ����
https://blog.csdn.net/jiangyu1013/article/details/78853407
git reset --merge 	�����˻�mergeǰ


"There is no tracking information for the current branch" �������
��ǰ��֧û�и�����Ϣ��
git branch --set-upstream-to=origin/���ط�֧


git reset HEAD^���ǽ�HEADָ��ǰ�ƣ�ָ����һ������
����
git log --graph --all	�����鿴�汾״̬
git log --graph --pretty=oneline --abbrev-commit �鿴�����汾�ߵ�״̬��
git status����״̬

��master��֧�Ͽ���һ���µ�develop��֧��Ȼ�����Ǹ��ݹ��ܻ���ҵ������develop
��֧�����⿪��������֧����ɷ�֧�ϵ�������ٽ������֧�ϲ���develop��֧�ϣ�
master��֧����ֱ�����ڲ�Ʒ�����Ĵ��룬������ʽ��Ĵ���
develop��֧���ճ������õķ�֧���Ŷ��е��˶��������֧�Ͻ��п���
��ʱ�Է�֧�������ض�Ŀ�Ŀ��ٵķ�֧����������(feature)��֧������Ԥ����(release)��֧��
�ֻ������޸�bug��fixbug����֧����ʱ�Է�֧����֮��һ�㶼��ɾ����ʹ�ô����ĳ��÷�֧ʼ��
ֻ���������ڷ�֧��


# package安装依赖

## 指定package安装依赖

```shell
# 推荐
$ lerna add lodash packages/module-1
# 或者
$ lerna add lodash --scope=module-1
# 或者
$ lerna add lodash **/module-1
# 或者
$ yarn workspace module-1 add lodash
```

## 给所有的package安装依赖

```shell
$ lerna add lodash
```

## workspace之间安装依赖

```shell
$ lerna add module-2 --scope module-1
# 或者
$ lerna add module-2 packages/module-1
```
# dddbook
# domain是核心业务领域，它不依赖任何其他服务，它使用抽象接口解耦服务的强依赖
# application 作为应用层(可以加入ACL防腐层)，依赖domain领域层 + 及基础设施层，它将基础设施作为输入，传入领域层进行处理，最后将数据返回出来，交由基础设施层进行处理
# domain领域层自洽，是最核心的业务逻辑，外层依赖内层；
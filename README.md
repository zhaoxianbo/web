获得原生类型的价值
如果value未定义或为null，则返回值较低的构造函数名称，“undefined”或“null”
const getType = v =>
  v === undefined ? 'undefined' : v === null ? 'null' : v.constructor.name.toLowerCase();

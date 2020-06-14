all:
	swiftc -emit-library -emit-module -I. -L. -module-name A DefaultInt.swift
	swiftc -emit-library -emit-module -I. -L. -module-name B FuncWithDefault.swift -lA
	swiftc -emit-library -emit-module -I. -L. -module-name C CallFuncWithDefault.swift -lB 2>&1 | swift demangle

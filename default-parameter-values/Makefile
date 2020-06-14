all:
	xcrun -sdk macosx swiftc -emit-library -emit-module -I. -L. -module-name A DefaultInt.swift
	xcrun -sdk macosx swiftc -emit-library -emit-module -I. -L. -module-name B FuncWithDefault.swift -lA
	xcrun -sdk macosx swiftc -emit-library -emit-module -I. -L. -module-name C CallFuncWithDefault.swift -lB 2>&1 | swift demangle

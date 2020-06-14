all:
	swiftc -emit-library -emit-module -I. -L. -module-name A Enum.swift
	swiftc -emit-library -emit-module -I. -L. -module-name B EnumArrayFunc.swift -lA
	swiftc -emit-library -emit-module -I. -L. -module-name C CallEnumArrayFunc.swift -lB 2>&1 | swift demangle

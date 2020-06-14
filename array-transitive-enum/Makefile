all:
	xcrun -sdk macosx xcrun -sdk macosx swiftc -emit-library -emit-module -I. -L. -module-name A Enum.swift
	xcrun -sdk macosx xcrun -sdk macosx swiftc -emit-library -emit-module -I. -L. -module-name B EnumArrayFunc.swift -lA
	xcrun -sdk macosx xcrun -sdk macosx swiftc -emit-library -emit-module -I. -L. -module-name C CallEnumArrayFunc.swift -lB 2>&1 | swift demangle

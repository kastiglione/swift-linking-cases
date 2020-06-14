all:
	xcrun -sdk macosx swiftc -emit-library -emit-module -I. -L. -module-name A BaseProtocol.swift
	xcrun -sdk macosx swiftc -emit-library -emit-module -I. -L. -module-name B Subprotocol.swift -lA
	xcrun -sdk macosx swiftc -emit-library -emit-module -I. -L. -module-name C Conformer.swift -lB 2>&1 | swift demangle

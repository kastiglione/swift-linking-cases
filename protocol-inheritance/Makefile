all:
	swiftc -emit-library -emit-module -I. -L. -module-name A BaseProtocol.swift
	swiftc -emit-library -emit-module -I. -L. -module-name B Subprotocol.swift -lA
	swiftc -emit-library -emit-module -I. -L. -module-name C Conformer.swift -lB

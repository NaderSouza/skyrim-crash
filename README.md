# skyrim-crash

Skyrim SSE v1.6.640
CrashLoggerSSE v1-10-0-0 Sep  5 2023 01:25:07

Unhandled exception "EXCEPTION_ACCESS_VIOLATION" at 0x7FF709BDDB5A SkyrimSE.exe+02EDB5A	mov rax, [rcx]

SYSTEM SPECS:
	OS: Microsoft Windows 11 Pro v10.0.22621
	CPU: AuthenticAMD AMD Ryzen 7 5800X 8-Core Processor             
	GPU #1: Nvidia TU104 [GeForce RTX 2060]
	GPU #2: Microsoft Basic Render Driver
	PHYSICAL MEMORY: 13.89 GB/15.90 GB
	GPU MEMORY: 3.26/5.07 GB

PROBABLE CALL STACK:
	[ 0] 0x7FF709BDDB5A SkyrimSE.exe+02EDB5A -> 21488+0x3A	mov rax, [rcx]
	[ 1] 0x7FF709D511EC SkyrimSE.exe+04611EC -> 29924+0x6BC	test al, al
	[ 2] 0x7FF709D500A4 SkyrimSE.exe+04600A4 -> 29895+0xE4	test byte ptr [rsi+0x30], 0x01
	[ 3] 0x7FF709C87F6D SkyrimSE.exe+0397F6D -> 25160+0x9D	test al, al
	[ 4] 0x7FF709C84861 SkyrimSE.exe+0394861 -> 25105+0xB1	mov esi, eax
	[ 5] 0x7FF709C80875 SkyrimSE.exe+0390875 -> 25063+0x15A5	mov ecx, eax
	[ 6] 0x7FF709C7D29D SkyrimSE.exe+038D29D -> 25048+0x1AD	mov ecx, [rax]
	[ 7] 0x7FF709DDF95C SkyrimSE.exe+04EF95C -> 32430+0xAC	test al, al
	[ 8] 0x7FF709DDEFA3 SkyrimSE.exe+04EEFA3 -> 32429+0xC3	mov r14d, eax
	[ 9] 0x7FF709DDECB6 SkyrimSE.exe+04EECB6 -> 32428+0x56	mov esi, eax
	[10] 0x7FF709DDECB6 SkyrimSE.exe+04EECB6 -> 32428+0x56	mov esi, eax
	[11] 0x7FF709DDECB6 SkyrimSE.exe+04EECB6 -> 32428+0x56	mov esi, eax
	[12] 0x7FF709DDCB11 SkyrimSE.exe+04ECB11 -> 32372+0x2D1	cmp eax, 0x01
	[13] 0x7FF709DE2DE0 SkyrimSE.exe+04F2DE0 -> 32483+0x380	xor sil, sil
	[14] 0x7FF709DE2A45 SkyrimSE.exe+04F2A45 -> 32482+0x15	mov rdx, rbx
	[15] 0x7FF709F68A56 SkyrimSE.exe+0678A56 -> 39060+0x36	nop
	[16] 0x7FF70A55C628 SkyrimSE.exe+0C6C628 -> 69378+0xD8	mov ecx, [rbx+0x0C]
	[17] 0x7FF70A55CBF1 SkyrimSE.exe+0C6CBF1 -> 69380+0x361	mov r15d, eax
	[18] 0x7FF70A55AF7A SkyrimSE.exe+0C6AF7A -> 69344+0x8A	movzx eax, byte ptr [rbx+0xA74]
	[19] 0x7FF70A535E4D SkyrimSE.exe+0C45E4D -> 68445+0x3D	mov rcx, [0x00007FF70C8F6898]
	[20] 0x7FFDCE6726AD KERNEL32.DLL+00126AD
	[21] 0x7FFDD016AA68    ntdll.dll+005AA68

REGISTERS:
	RAX 0x7FF709BDDB20     (void* -> SkyrimSE.exe+02EDB20	mov [rsp+0x08], rbx)
	RCX 0x0                (size_t) [0]
	RDX 0x1A2C1852750      (BGSListForm*)
		File: "Skyrim.esm"
		Flags: 0x00000009 kDestructible | kInitialized
		FormID: 0x000400B7
		FormType: FormList (91)
	RBX 0x1A2C1852750      (BGSListForm*)
		File: "Skyrim.esm"
		Flags: 0x00000009 kDestructible | kInitialized
		FormID: 0x000400B7
		FormType: FormList (91)
	RSP 0x4BF27FE580       (void*)
	RBP 0x4BF27FE679       (void*)
	RSI 0x1A2C83A5760      (TESObjectREFR*)
		Object Reference: None
		File: "Lux - JK's Blue Palace patch.esp"
		Modified by: JK's Blue Palace.esp -> Lux - JK's Blue Palace patch.esp
		Flags: 0x00000008 kInitialized
		FormID: 0x19042CB2
		FormType: Reference (61)
	RDI 0x4BF27FE620       (void*)
	R8  0x0                (size_t) [0]
	R9  0x4BF27FE620       (void*)
	R10 0x546C6148         (size_t) [1416388936]
	R11 0xFFFFFFFFFA905A89 (size_t) [uint: 18446744073618348681 int: -91202935]
	R12 0xFFFFFFFF         (size_t) [4294967295]
	R13 0x1A2C3624358      (void*)
	R14 0x0                (size_t) [0]
	R15 0x7FF70C88AA20     (void* -> SkyrimSE.exe+2F9AA20	)

STACK:
	[RSP+0   ] 0x1A2C1852750      (BGSListForm*)
		File: "Skyrim.esm"
		Flags: 0x00000009 kDestructible | kInitialized
		FormID: 0x000400B7
		FormType: FormList (91)
	[RSP+8   ] 0x4BF27FE679       (void*)
	[RSP+10  ] 0x1A2C83C6AC0      (TESObjectREFR*)
		Object Reference: 
		File: "Skyrim.esm"
		Flags: 0x00000009 kDestructible | kInitialized
		FormID: 0x0005EF8F
		FormType: Static (34)
		File: "JK's Blue Palace.esp"
		Flags: 0x00000408 kInitialized
		FormID: 0x1903D86D
		FormType: Reference (61)
	[RSP+18  ] 0x4BF27FE620       (void*)
	[RSP+20  ] 0x1A2C83A5760      (TESObjectREFR*)
		Object Reference: None
		File: "Lux - JK's Blue Palace patch.esp"
		Modified by: JK's Blue Palace.esp -> Lux - JK's Blue Palace patch.esp
		Flags: 0x00000008 kInitialized
		FormID: 0x19042CB2
		FormType: Reference (61)
	[RSP+28  ] 0x7FF709D511EC     (void* -> SkyrimSE.exe+04611EC	test al, al)
	[RSP+30  ] 0x0                (size_t) [0]
	[RSP+38  ] 0x1A2C1852750      (BGSListForm*)
		File: "Skyrim.esm"
		Flags: 0x00000009 kDestructible | kInitialized
		FormID: 0x000400B7
		FormType: FormList (91)
	[RSP+40  ] 0x1A2C186BC40      (BGSListForm*)
		File: "Skyrim.esm"
		Flags: 0x00000009 kDestructible | kInitialized
		FormID: 0x000F9073
		FormType: FormList (91)
	[RSP+48  ] 0x1A2BA501600      (Character*)
		File: "JK's Blue Palace.esp"
		Modified by: Skyrim.esm -> JK's Blue Palace.esp
		Flags: 0x00000409 
		Name: "Bolgeir Bearclaw"
		FormID: 0x000198C3
		FormType: ActorCharacter (62)
		Object Reference: 
		File: "Unofficial Skyrim Special Edition Patch.esp"
		Modified by: Skyrim.esm -> Unofficial Skyrim Special Edition Patch.esp
		Flags: 0x00040009 kDestructible | kInitialized
		Name: "Bolgeir Bearclaw"
		FormID: 0x00013264
		FormType: NPC (43)
		File: "JK's Blue Palace.esp"
		Modified by: Skyrim.esm -> JK's Blue Palace.esp
		Flags: 0x00000409 kDestructible | kInitialized
		FormID: 0x000198C3
		FormType: ActorCharacter (62)
	[RSP+50  ] 0x0                (size_t) [0]
	[RSP+58  ] 0x7FFD883657C3     (void* -> tbbmalloc.dll+00157C3	mov rbp, rax)
	[RSP+60  ] 0x0                (size_t) [0]
	[RSP+68  ] 0x4BF27FEF20       (char*) " "
	[RSP+70  ] 0x4BF27FE740       (void*)
	[RSP+78  ] 0x7FF70A5514E2     (void* -> SkyrimSE.exe+0C614E2	nop)
	[RSP+80  ] 0x4BF27FEED8       (void*)
	[RSP+88  ] 0x7FF70AC4FB48     (void* -> SkyrimSE.exe+135FB48	jmp 0x00007FF70AC4FB86)
	[RSP+90  ] 0x1A39B9EE390      (BSScript::Internal::CodeTasklet*)
		Stack Trace: 
[None].xpmselib.SetNodeParent() - "XPMSELib.psc" Line 0
[None].XPMSEWeaponStyleScaleEffect.SetNodeParent() - "XPMSEWeaponStyleScaleEffect.psc" Line 0
[None].XPMSEWeaponStyleScaleEffect.CleanupStyle() - "XPMSEWeaponStyleScaleEffect.psc" Line 0
[None].XPMSEWeaponStyleScaleEffect.CleanupAll() - "XPMSEWeaponStyleScaleEffect.psc" Line 0
[None].XPMSEWeaponStyleScaleEffect.OnUnload() - "XPMSEWeaponStyleScaleEffect.psc" Line 0

	[RSP+98  ] 0x7FF70AC93A8C     (void* -> SkyrimSE.exe+13A3A8C	movzx eax, r15b)
	[RSP+A0  ] 0x0                (size_t) [0]
	[RSP+A8  ] 0x0                (size_t) [0]
	[RSP+B0  ] 0x0                (size_t) [0]
	[RSP+B8  ] 0x7FF70AC9383A     (void* -> SkyrimSE.exe+13A383A	jmp 0x00007FF70AC93A8C)
	[RSP+C0  ] 0x1A39B9EE390      (BSScript::Internal::CodeTasklet*)
		Stack Trace: 
[None].xpmselib.SetNodeParent() - "XPMSELib.psc" Line 0
[None].XPMSEWeaponStyleScaleEffect.SetNodeParent() - "XPMSEWeaponStyleScaleEffect.psc" Line 0
[None].XPMSEWeaponStyleScaleEffect.CleanupStyle() - "XPMSEWeaponStyleScaleEffect.psc" Line 0
[None].XPMSEWeaponStyleScaleEffect.CleanupAll() - "XPMSEWeaponStyleScaleEffect.psc" Line 0
[None].XPMSEWeaponStyleScaleEffect.OnUnload() - "XPMSEWeaponStyleScaleEffect.psc" Line 0

	[RSP+C8  ] 0x7FFD88363911     (void* -> tbbmalloc.dll+0013911	xor ecx, ecx)
	[RSP+D0  ] 0x4BF27FE6B0       (void*)
	[RSP+D8  ] 0x1                (size_t) [1]
	[RSP+E0  ] 0x4                (size_t) [4]
	[RSP+E8  ] 0xFFFFFFFFFFFFFFFE (size_t) [uint: 18446744073709551614 int: -2]
	[RSP+F0  ] 0x8                (size_t) [8]
	[RSP+F8  ] 0x40               (size_t) [64]
	[RSP+100 ] 0x40000000         (size_t) [1073741824]
	[RSP+108 ] 0x0                (size_t) [0]
	[RSP+110 ] 0x4BF27FE6B0       (void*)
	[RSP+118 ] 0x0                (size_t) [0]
	[RSP+120 ] 0x7FF70C88AA00     (void* -> SkyrimSE.exe+2F9AA00	add [rax], al)
	[RSP+128 ] 0x1A22F3CE590      (void*)
	[RSP+130 ] 0x0                (size_t) [0]
	[RSP+138 ] 0x7FF70C88AA20     (void* -> SkyrimSE.exe+2F9AA20	)
	[RSP+140 ] 0x1A2C3624340      (void*)
	[RSP+148 ] 0x1A2C9128801      (void*)
	[RSP+150 ] 0x1A2C913C900      (void*)
	[RSP+158 ] 0x7FF709D500A4     (void* -> SkyrimSE.exe+04600A4	test byte ptr [rsi+0x30], 0x01)
	[RSP+160 ] 0x1A2C3624340      (void*)
	[RSP+168 ] 0x7FFD00000000     (size_t) [140724603453440]
	[RSP+170 ] 0x7FF70C88AA20     (void* -> SkyrimSE.exe+2F9AA20	)
	[RSP+178 ] 0x0                (size_t) [0]
	[RSP+180 ] 0x1A22F3CE5B8      (void*)
	[RSP+188 ] 0x0                (size_t) [0]
	[RSP+190 ] 0x1A22F3CE5B0      (void*)
	[RSP+198 ] 0x0                (size_t) [0]
	[RSP+1A0 ] 0x1                (size_t) [1]
	[RSP+1A8 ] 0x7FF70C88AA20     (void* -> SkyrimSE.exe+2F9AA20	)
	[RSP+1B0 ] 0x33B              (size_t) [827]
	[RSP+1B8 ] 0x1                (size_t) [1]
	[RSP+1C0 ] 0x1A2C913C9C0      (void*)
	[RSP+1C8 ] 0x1A2C83A5760      (TESObjectREFR*)
		Object Reference: None
		File: "Lux - JK's Blue Palace patch.esp"
		Modified by: JK's Blue Palace.esp -> Lux - JK's Blue Palace patch.esp
		Flags: 0x00000008 kInitialized
		FormID: 0x19042CB2
		FormType: Reference (61)
	[RSP+1D0 ] 0x1A2C9128860      (void*)
	[RSP+1D8 ] 0x7FF709C87F6D     (void* -> SkyrimSE.exe+0397F6D	test al, al)
	[RSP+1E0 ] 0x0                (size_t) [0]
	[RSP+1E8 ] 0x1A22F3CE5C0      (void*)
	[RSP+1F0 ] 0x1A2C913C9C0      (void*)
	[RSP+1F8 ] 0x0                (size_t) [0]
	[RSP+200 ] 0xFFFFFFFFFFFFFFFE (size_t) [uint: 18446744073709551614 int: -2]
	[RSP+208 ] 0x7FF70AF0A598     (void* -> SkyrimSE.exe+161A598	nop)
	[RSP+210 ] 0x7FF70C88AA88     (void* -> SkyrimSE.exe+2F9AA88	sbb byte ptr [rcx], 0xB5)
	[RSP+218 ] 0x7FF709A460EE     (void* -> SkyrimSE.exe+01560EE	mov ebp, eax)
	[RSP+220 ] 0x0                (size_t) [0]
	[RSP+228 ] 0x7FF70C88AA20     (void* -> SkyrimSE.exe+2F9AA20	)
	[RSP+230 ] 0x33B              (size_t) [827]
	[RSP+238 ] 0x1                (size_t) [1]
	[RSP+240 ] 0x1A2C913C9C0      (void*)
	[RSP+248 ] 0x7FF709C84861     (void* -> SkyrimSE.exe+0394861	mov esi, eax)
	[RSP+250 ] 0x18A              (size_t) [394]
	[RSP+258 ] 0x1A2C9128860      (void*)
	[RSP+260 ] 0x1                (size_t) [1]
	[RSP+268 ] 0x1A2BA4F3700      (TESObjectCELL*)
		File: "Lux - JK's Blue Palace patch.esp"
		Modified by: Skyrim.esm -> Unofficial Skyrim Special Edition Patch.esp -> 3DNPC.esp -> Book Covers Skyrim.esp -> JK's Blue Palace.esp -> PrvtIRoyalArmory.esp -> Lux.esp -> JKs Blue Palace - Immersion Patch.esp -> Lux - JK's Blue Palace patch.esp
		Flags: 0x00040009 
		Name: "Blue Palace"
		EditorID: "SolitudeBluePalace"
		FormID: 0x00016A04
		FormType: Cell (60)
		File: "Lux - JK's Blue Palace patch.esp"
		Modified by: Skyrim.esm -> Unofficial Skyrim Special Edition Patch.esp -> 3DNPC.esp -> Book Covers Skyrim.esp -> JK's Blue Palace.esp -> PrvtIRoyalArmory.esp -> Lux.esp -> JKs Blue Palace - Immersion Patch.esp -> Lux - JK's Blue Palace patch.esp
		Flags: 0x00040009 kDestructible | kInitialized
		Name: "Blue Palace"
		EditorID: "SolitudeBluePalace"
		FormID: 0x00016A04
		FormType: Cell (60)
		GetFullName: "Blue Palace"
	[RSP+270 ] 0xFFFFFFFFFFFFFFFE (size_t) [uint: 18446744073709551614 int: -2]
	[RSP+278 ] 0x4BF4A39070A32854 (size_t) [5473179287922354260]
	[RSP+280 ] 0x1A2C772A1B0      (BGSRefAlias*)
	[RSP+288 ] 0x0                (size_t) [0]
	[RSP+290 ] 0x7FF70B84CA40     (void* -> SkyrimSE.exe+1F5CA40	add [rax], al)
	[RSP+298 ] 0xC50              (size_t) [3152]
	[RSP+2A0 ] 0x7FF70C88AA20     (void* -> SkyrimSE.exe+2F9AA20	)
	[RSP+2A8 ] 0x7FF709C80875     (void* -> SkyrimSE.exe+0390875	mov ecx, eax)
	[RSP+2B0 ] 0x1A2BA4F3820      (void*)
	[RSP+2B8 ] 0x18A              (size_t) [394]
	[RSP+2C0 ] 0x4BF27FE930       (void*)
	[RSP+2C8 ] 0x0                (size_t) [0]
	[RSP+2D0 ] 0x4BF27FF2E0       (void*)
	[RSP+2D8 ] 0x4BF27FF2F0       (void*)
	[RSP+2E0 ] 0x32C000001        (size_t) [13623099393]
	[RSP+2E8 ] 0x4BF27FE880       (void*)
	[RSP+2F0 ] 0x7FFF7FFF         (size_t) [2147450879]
	[RSP+2F8 ] 0x7FF70C8E1570     (void* -> SkyrimSE.exe+2FF1570	call 0x00007FF78C852085)
	[RSP+300 ] 0x1A20E518BF0      (void*)
	[RSP+308 ] 0x8000000100000000 (size_t) [uint: 9223372041149743104 int: -9223372032559808512]
	[RSP+310 ] 0x1A20E518BF0      (void*)
	[RSP+318 ] 0x7FF700000001     (size_t) [140698833649665]
	[RSP+320 ] 0x32C95BD01        (size_t) [13632912641]
	[RSP+328 ] 0x4BF27FF2F8       (void*)
	[RSP+330 ] 0x0                (size_t) [0]
	[RSP+338 ] 0xFFFFFFFFFFFFFFFE (size_t) [uint: 18446744073709551614 int: -2]
	[RSP+340 ] 0x1A22C6AF400      (hkbStateMachine*)
		Name: "RootBehaviorGraph"
		ID: 0x0000004A
	[RSP+348 ] 0x0                (size_t) [0]
	[RSP+350 ] 0x0                (size_t) [0]
	[RSP+358 ] 0x0                (size_t) [0]
	[RSP+360 ] 0x7FFFFFFF         (size_t) [2147483647]
	[RSP+368 ] 0x0                (size_t) [0]
	[RSP+370 ] 0x7FF70B84CA40     (void* -> SkyrimSE.exe+1F5CA40	add [rax], al)
	[RSP+378 ] 0xFFFFFFFFFFFFFFFE (size_t) [uint: 18446744073709551614 int: -2]
	[RSP+380 ] 0x0                (size_t) [0]
	[RSP+388 ] 0x0                (size_t) [0]
	[RSP+390 ] 0x0                (size_t) [0]
	[RSP+398 ] 0x0                (size_t) [0]
	[RSP+3A0 ] 0x7FFFFFFF         (size_t) [2147483647]
	[RSP+3A8 ] 0x0                (size_t) [0]
	[RSP+3B0 ] 0x3C89E60F         (size_t) [1015670287]
	[RSP+3B8 ] 0x0                (size_t) [0]
	[RSP+3C0 ] 0x0                (size_t) [0]
	[RSP+3C8 ] 0x4BF27FF3C8       (void*)
	[RSP+3D0 ] 0x4BF27FF2E0       (void*)
	[RSP+3D8 ] 0x4BF27FF3D8       (void*)
	[RSP+3E0 ] 0x1A22C6AF900      (hkbBehaviorGraph*)
		Name: "0_Master.hkb"
		ID: 0x0000FFFF
	[RSP+3E8 ] 0x4BF27FF330       (void*)
	[RSP+3F0 ] 0x0                (size_t) [0]
	[RSP+3F8 ] 0x7FF70A48F79D     (void* -> SkyrimSE.exe+0B9F79D	mov rcx, rax)
	[RSP+400 ] 0x0                (size_t) [0]
	[RSP+408 ] 0x4BF27FEA80       (void*)
	[RSP+410 ] 0x4BF27FF3D8       (void*)
	[RSP+418 ] 0x0                (size_t) [0]
	[RSP+420 ] 0x4BF27FF2E0       (void*)
	[RSP+428 ] 0x4BF27FF2F0       (void*)
	[RSP+430 ] 0x7FF70C88AA20     (void* -> SkyrimSE.exe+2F9AA20	)
	[RSP+438 ] 0x4BF27FE9D0       (void*)
	[RSP+440 ] 0x10000            (size_t) [65536]
	[RSP+448 ] 0x7FF70C8E7860     (void* -> SkyrimSE.exe+2FF7860	mov al, 0xD0)
	[RSP+450 ] 0x1A20E518B70      (void*)
	[RSP+458 ] 0x8000000100000000 (size_t) [uint: 9223372041149743104 int: -9223372032559808512]
	[RSP+460 ] 0xFFFFFFFFFFFFFFFE (size_t) [uint: 18446744073709551614 int: -2]
	[RSP+468 ] 0x7FF700000001     (size_t) [140698833649665]
	[RSP+470 ] 0x1A2CAA34180      (TESObjectREFR*)
		Object Reference: 
		File: "Skyrim.esm"
		Flags: 0x00020009 kDestructible | kInitialized
		FormID: 0x000B33F0
		FormType: Light (31)
		File: "Lux.esp"
		Flags: 0x00000C08 kInitialized
		FormID: 0x000A5804
		FormType: Reference (61)
	[RSP+478 ] 0x7FF70A55276D     (void* -> SkyrimSE.exe+0C6276D	mov r13, rax)
	[RSP+480 ] 0xFFFFFFFFFFFFFFFE (size_t) [uint: 18446744073709551614 int: -2]
	[RSP+488 ] 0xFFFFFFFFFFFFFFFE (size_t) [uint: 18446744073709551614 int: -2]
	[RSP+490 ] 0x4BF27FEB38       (void*)
	[RSP+498 ] 0x7FF70A55276D     (void* -> SkyrimSE.exe+0C6276D	mov r13, rax)
	[RSP+4A0 ] 0xFFFFFFFFFFFFFFFE (size_t) [uint: 18446744073709551614 int: -2]
	[RSP+4A8 ] 0x1A2A767C8E0      (void*)
	[RSP+4B0 ] 0xFFFFFFFFFFFFFFFE (size_t) [uint: 18446744073709551614 int: -2]
	[RSP+4B8 ] 0x1A22F3CE6D8      (char*) "o"
	[RSP+4C0 ] 0x4BF27FF398       (void*)
	[RSP+4C8 ] 0x7FF70A55276D     (void* -> SkyrimSE.exe+0C6276D	mov r13, rax)
	[RSP+4D0 ] 0x1                (size_t) [1]
	[RSP+4D8 ] 0x4BF27FF440       (char*) "?"
	[RSP+4E0 ] 0x1A38EF45A80      (BSTriShape*)
		Name: "WRdragonDoorNewR:16"
		RTTIName: "BSTriShape"
		Flags: kSelectiveUpdate | kSelectiveUpdateTransforms | kSelectiveUpdateController
		Full Name: "Porta"
		File: "Architecture\WhiteRun\WRDragonDoor01.nif"
		Checking Owner: -----
			File: "Unofficial Skyrim Special Edition Patch.esp"
			Modified by: Skyrim.esm -> Unofficial Skyrim Special Edition Patch.esp
			Flags: 0x00000009 kDestructible | kInitialized
			Name: "Whiterun Bannered Mare Faction"
			FormID: 0x0009E1B4
			FormType: Faction (11)
		Checking User Data: -----
			Object Reference: 
			File: "Skyrim.esm"
			Flags: 0x00000009 kDestructible | kInitialized
			Name: "Porta"
			FormID: 0x000252C7
			FormType: Door (29)
		Checking TESObjectREFR: {}
			Object Reference: 
			File: "Skyrim.esm"
			Flags: 0x00000009 kDestructible | kInitialized
			Name: "Porta"
			FormID: 0x000252C7
			FormType: Door (29)
		Checking Parent: 1
			Name: "WRdragonDoorNewR"
			RTTIName: "NiNode"
			Flags: kSelectiveUpdate | kSelectiveUpdateTransforms | kSelectiveUpdateController | kSelectiveUpdateTransformsOverride
			Full Name: "Porta"
			File: "Architecture\WhiteRun\WRDragonDoor01.nif"
			Checking Owner: -----
				File: "Unofficial Skyrim Special Edition Patch.esp"
				Modified by: Skyrim.esm -> Unofficial Skyrim Special Edition Patch.esp
				Flags: 0x00000009 kDestructible | kInitialized
				Name: "Whiterun Bannered Mare Faction"
				FormID: 0x0009E1B4
				FormType: Faction (11)
			Checking User Data: -----
				Object Reference: 
				File: "Skyrim.esm"
				Flags: 0x00000009 kDestructible | kInitialized
				Name: "Porta"
				FormID: 0x000252C7
				FormType: Door (29)
			Checking TESObjectREFR: {}
				Object Reference: 
				File: "Skyrim.esm"
				Flags: 0x00000009 kDestructible | kInitialized
				Name: "Porta"
				FormID: 0x000252C7
				FormType: Door (29)
			Checking Parent: 0
				Name: "DoorRDummy"
				RTTIName: "NiNode"
				Flags: kSelectiveUpdate | kSelectiveUpdateTransforms | kSelectiveUpdateController
				Full Name: "Porta"
				File: "Architecture\WhiteRun\WRDragonDoor01.nif"
				Checking Owner: -----
					File: "Unofficial Skyrim Special Edition Patch.esp"
					Modified by: Skyrim.esm -> Unofficial Skyrim Special Edition Patch.esp
					Flags: 0x00000009 kDestructible | kInitialized
					Name: "Whiterun Bannered Mare Faction"
					FormID: 0x0009E1B4
					FormType: Faction (11)
				Checking User Data: -----
					Object Reference: 
					File: "Skyrim.esm"
					Flags: 0x00000009 kDestructible | kInitialized
					Name: "Porta"
					FormID: 0x000252C7
					FormType: Door (29)
				Checking TESObjectREFR: {}
					Object Reference: 
					File: "Skyrim.esm"
					Flags: 0x00000009 kDestructible | kInitialized
					Name: "Porta"
					FormID: 0x000252C7
					FormType: Door (29)
				Checking Parent: 1
					Name: "WRDragonDoor01"
					RTTIName: "BSFadeNode"
					ExtraData[0] Name: "BSX"
					Flags: kSelectiveUpdate | kSelectiveUpdateTransforms | kSelectiveUpdateController
					Full Name: "Porta"
					File: "Architecture\WhiteRun\WRDragonDoor01.nif"
					Checking Owner: -----
						File: "Unofficial Skyrim Special Edition Patch.esp"
						Modified by: Skyrim.esm -> Unofficial Skyrim Special Edition Patch.esp
						Flags: 0x00000009 kDestructible | kInitialized
						Name: "Whiterun Bannered Mare Faction"
						FormID: 0x0009E1B4
						FormType: Faction (11)
					Checking User Data: -----
						Object Reference: 
						File: "Skyrim.esm"
						Flags: 0x00000009 kDestructible | kInitialized
						Name: "Porta"
						FormID: 0x000252C7
						FormType: Door (29)
					Checking TESObjectREFR: {}
						Object Reference: 
						File: "Skyrim.esm"
						Flags: 0x00000009 kDestructible | kInitialized
						Name: "Porta"
						FormID: 0x000252C7
						FormType: Door (29)
					Checking Parent: 53
						RTTIName: "NiNode"
						Flags: kSelectiveUpdate | kSelectiveUpdateTransforms | kSelectiveUpdateController
						Checking Parent: 3
							RTTIName: "BSMultiBoundNode"
							Flags: kSelectiveUpdate | kSelectiveUpdateTransforms | kSelectiveUpdateController
							Checking Parent: 25
								Name: "ObjectLODRoot"
								RTTIName: "NiNode"
								Flags: kSelectiveUpdate | kSelectiveUpdateTransforms | kSelectiveUpdateController
								Checking Parent: 3
									Name: "shadow scene node"
									RTTIName: "ShadowSceneNode"
									Flags: kSelectiveUpdate | kSelectiveUpdateTransforms | kSelectiveUpdateController
									Checking Parent: 1
										Name: "WorldRoot Node"
										RTTIName: "SceneGraph"
										Flags: kSelectiveUpdate | kSelectiveUpdateTransforms | kSelectiveUpdateController
		Name: "WRdragonDoorNewR:16"
	[RSP+4E8 ] 0x7FF70A69440F     (void* -> SkyrimSE.exe+0DA440F	nop)
	[RSP+4F0 ] 0xFFFFFFFFFFFFFFFE (size_t) [uint: 18446744073709551614 int: -2]
	[RSP+4F8 ] 0x1A22F3CE6D8      (char*) "o"
	[RSP+500 ] 0x1                (size_t) [1]
	[RSP+508 ] 0x4BF27FF440       (char*) "?"
	[RSP+510 ] 0xFFFFFFFFFFFFFFFE (size_t) [uint: 18446744073709551614 int: -2]
	[RSP+518 ] 0x7FF70AF0A598     (void* -> SkyrimSE.exe+161A598	nop)
	[RSP+520 ] 0x1A236EF19A8      (void*)
	[RSP+528 ] 0x7FF70AC4FCFC     (void* -> SkyrimSE.exe+135FCFC	test eax, eax)
	[RSP+530 ] 0x1A22F3CE6D8      (char*) "o"
	[RSP+538 ] 0x7FF70A59C998     (void* -> SkyrimSE.exe+0CAC998	nop)
	[RSP+540 ] 0x20               (size_t) [32]
	[RSP+548 ] 0xFFFFFFFF         (size_t) [4294967295]
	[RSP+550 ] 0xFFFFFFFFFFFFFFFE (size_t) [uint: 18446744073709551614 int: -2]
	[RSP+558 ] 0x1A22C688C00      (hkbManualSelectorGenerator*)
		Name: "1st3rdPerson_MSG"
		ID: 0x00000045
	[RSP+560 ] 0xFFFFFFFFFFFFFFFE (size_t) [uint: 18446744073709551614 int: -2]
	[RSP+568 ] 0x0                (size_t) [0]
	[RSP+570 ] 0x1A236EF1880      (BSGeometryListCullingProcess*)
	[RSP+578 ] 0x7FF70A68C421     (void* -> SkyrimSE.exe+0D9C421	mov [rdi+0x9C], r14d)
	[RSP+580 ] 0x1A300000020      (void*)
	[RSP+588 ] 0x1A38EF45A80      (BSTriShape*)
		Name: "WRdragonDoorNewR:16"
		RTTIName: "BSTriShape"
		Flags: kSelectiveUpdate | kSelectiveUpdateTransforms | kSelectiveUpdateController
		Full Name: "Porta"
		File: "Architecture\WhiteRun\WRDragonDoor01.nif"
		Checking Owner: -----
			File: "Unofficial Skyrim Special Edition Patch.esp"
			Modified by: Skyrim.esm -> Unofficial Skyrim Special Edition Patch.esp
			Flags: 0x00000009 kDestructible | kInitialized
			Name: "Whiterun Bannered Mare Faction"
			FormID: 0x0009E1B4
			FormType: Faction (11)
		Checking User Data: -----
			Object Reference: 
			File: "Skyrim.esm"
			Flags: 0x00000009 kDestructible | kInitialized
			Name: "Porta"
			FormID: 0x000252C7
			FormType: Door (29)
		Checking TESObjectREFR: {}
			Object Reference: 
			File: "Skyrim.esm"
			Flags: 0x00000009 kDestructible | kInitialized
			Name: "Porta"
			FormID: 0x000252C7
			FormType: Door (29)
		Checking Parent: 1
			Name: "WRdragonDoorNewR"
			RTTIName: "NiNode"
			Flags: kSelectiveUpdate | kSelectiveUpdateTransforms | kSelectiveUpdateController | kSelectiveUpdateTransformsOverride
			Full Name: "Porta"
			File: "Architecture\WhiteRun\WRDragonDoor01.nif"
			Checking Owner: -----
				File: "Unofficial Skyrim Special Edition Patch.esp"
				Modified by: Skyrim.esm -> Unofficial Skyrim Special Edition Patch.esp
				Flags: 0x00000009 kDestructible | kInitialized
				Name: "Whiterun Bannered Mare Faction"
				FormID: 0x0009E1B4
				FormType: Faction (11)
			Checking User Data: -----
				Object Reference: 
				File: "Skyrim.esm"
				Flags: 0x00000009 kDestructible | kInitialized
				Name: "Porta"
				FormID: 0x000252C7
				FormType: Door (29)
			Checking TESObjectREFR: {}
				Object Reference: 
				File: "Skyrim.esm"
				Flags: 0x00000009 kDestructible | kInitialized
				Name: "Porta"
				FormID: 0x000252C7
				FormType: Door (29)
			Checking Parent: 0
				Name: "DoorRDummy"
				RTTIName: "NiNode"
				Flags: kSelectiveUpdate | kSelectiveUpdateTransforms | kSelectiveUpdateController
				Full Name: "Porta"
				File: "Architecture\WhiteRun\WRDragonDoor01.nif"
				Checking Owner: -----
					File: "Unofficial Skyrim Special Edition Patch.esp"
					Modified by: Skyrim.esm -> Unofficial Skyrim Special Edition Patch.esp
					Flags: 0x00000009 kDestructible | kInitialized
					Name: "Whiterun Bannered Mare Faction"
					FormID: 0x0009E1B4
					FormType: Faction (11)
				Checking User Data: -----
					Object Reference: 
					File: "Skyrim.esm"
					Flags: 0x00000009 kDestructible | kInitialized
					Name: "Porta"
					FormID: 0x000252C7
					FormType: Door (29)
				Checking TESObjectREFR: {}
					Object Reference: 
					File: "Skyrim.esm"
					Flags: 0x00000009 kDestructible | kInitialized
					Name: "Porta"
					FormID: 0x000252C7
					FormType: Door (29)
				Checking Parent: 1
					Name: "WRDragonDoor01"
					RTTIName: "BSFadeNode"
					ExtraData[0] Name: "BSX"
					Flags: kSelectiveUpdate | kSelectiveUpdateTransforms | kSelectiveUpdateController
					Full Name: "Porta"
					File: "Architecture\WhiteRun\WRDragonDoor01.nif"
					Checking Owner: -----
						File: "Unofficial Skyrim Special Edition Patch.esp"
						Modified by: Skyrim.esm -> Unofficial Skyrim Special Edition Patch.esp
						Flags: 0x00000009 kDestructible | kInitialized
						Name: "Whiterun Bannered Mare Faction"
						FormID: 0x0009E1B4
						FormType: Faction (11)
					Checking User Data: -----
						Object Reference: 
						File: "Skyrim.esm"
						Flags: 0x00000009 kDestructible | kInitialized
						Name: "Porta"
						FormID: 0x000252C7
						FormType: Door (29)
					Checking TESObjectREFR: {}
						Object Reference: 
						File: "Skyrim.esm"
						Flags: 0x00000009 kDestructible | kInitialized
						Name: "Porta"
						FormID: 0x000252C7
						FormType: Door (29)
					Checking Parent: 53
						RTTIName: "NiNode"
						Flags: kSelectiveUpdate | kSelectiveUpdateTransforms | kSelectiveUpdateController
						Checking Parent: 3
							RTTIName: "BSMultiBoundNode"
							Flags: kSelectiveUpdate | kSelectiveUpdateTransforms | kSelectiveUpdateController
							Checking Parent: 25
								Name: "ObjectLODRoot"
								RTTIName: "NiNode"
								Flags: kSelectiveUpdate | kSelectiveUpdateTransforms | kSelectiveUpdateController
								Checking Parent: 3
									Name: "shadow scene node"
									RTTIName: "ShadowSceneNode"
									Flags: kSelectiveUpdate | kSelectiveUpdateTransforms | kSelectiveUpdateController
									Checking Parent: 1
										Name: "WorldRoot Node"
										RTTIName: "SceneGraph"
										Flags: kSelectiveUpdate | kSelectiveUpdateTransforms | kSelectiveUpdateController
		Name: "WRdragonDoorNewR:16"
	[RSP+590 ] 0x1A3A1DBF400      (void*)
	[RSP+598 ] 0x1A3A1BFDC10      (BSScript::Internal::CodeTasklet*)
		Stack Trace: 
[None].xpmselib.SetNodeScaleSkeleton() - "XPMSELib.psc" Line 0
[None].XPMSEWeaponStyleScaleEffect.SetNodeScale() - "XPMSEWeaponStyleScaleEffect.psc" Line 0
[None].XPMSEWeaponStyleScaleEffect.CleanupScale() - "XPMSEWeaponStyleScaleEffect.psc" Line 0
[None].XPMSEWeaponStyleScaleEffect.CleanupAll() - "XPMSEWeaponStyleScaleEffect.psc" Line 0
[None].XPMSEWeaponStyleScaleEffect.OnCellDetach() - "XPMSEWeaponStyleScaleEffect.psc" Line 0

	[RSP+5A0 ] 0xF0000003F        (size_t) [64424509503]
	[RSP+5A8 ] 0x2300000003       (size_t) [150323855363]
	[RSP+5B0 ] 0x3F00000003       (size_t) [270582939651]
	[RSP+5B8 ] 0x2F00000003       (size_t) [201863462915]
	[RSP+5C0 ] 0x3F00000003       (size_t) [270582939651]
	[RSP+5C8 ] 0x3C00000003       (size_t) [257698037763]
	[RSP+5D0 ] 0x3E00000003       (size_t) [266287972355]
	[RSP+5D8 ] 0x3E00000003       (size_t) [266287972355]
	[RSP+5E0 ] 0x1E00000003       (size_t) [128849018883]
	[RSP+5E8 ] 0xE00000003        (size_t) [60129542147]
	[RSP+5F0 ] 0x3C00000003       (size_t) [257698037763]
	[RSP+5F8 ] 0x300000034        (size_t) [12884901940]
	[RSP+600 ] 0x30000003E        (size_t) [12884901950]
	[RSP+608 ] 0x3F0000003D       (size_t) [270582939709]
	[RSP+610 ] 0x3F00000003       (size_t) [270582939651]
	[RSP+618 ] 0x3E00000003       (size_t) [266287972355]
	[RSP+620 ] 0x3E00000003       (size_t) [266287972355]
	[RSP+628 ] 0x1000000003       (size_t) [68719476739]
	[RSP+630 ] 0x3E00000000       (size_t) [266287972352]
	[RSP+638 ] 0x3C00000003       (size_t) [257698037763]
	[RSP+640 ] 0x1E00000003       (size_t) [128849018883]
	[RSP+648 ] 0x3                (size_t) [3]
	[RSP+650 ] 0x3C89E60F         (size_t) [1015670287]
	[RSP+658 ] 0x0                (size_t) [0]
	[RSP+660 ] 0x0                (size_t) [0]
	[RSP+668 ] 0x4BF27FF3C8       (void*)
	[RSP+670 ] 0x4BF27FF2E0       (void*)
	[RSP+678 ] 0x4BF27FF3D8       (void*)
	[RSP+680 ] 0x1A22C6AF900      (hkbBehaviorGraph*)
		Name: "0_Master.hkb"
		ID: 0x0000FFFF
	[RSP+688 ] 0x4BF27FF330       (void*)
	[RSP+690 ] 0x4BF27FED20       (void*)
	[RSP+698 ] 0x7FF70A48F79D     (void* -> SkyrimSE.exe+0B9F79D	mov rcx, rax)
	[RSP+6A0 ] 0x0                (size_t) [0]
	[RSP+6A8 ] 0x1A22C688E40      (hkbManualSelectorGenerator*)
		Name: "DualWieldShieldBoneRootMSG"
		ID: 0x0000001C
	[RSP+6B0 ] 0x4BF27FF3D8       (void*)
	[RSP+6B8 ] 0x0                (size_t) [0]
	[RSP+6C0 ] 0x4BF27FF2E0       (void*)
	[RSP+6C8 ] 0x4BF27FF2F0       (void*)
	[RSP+6D0 ] 0x44560C6F00000001 (size_t) [4924136913457119233]
	[RSP+6D8 ] 0x4BF27FEC70       (void*)
	[RSP+6E0 ] 0x0                (size_t) [0]
	[RSP+6E8 ] 0x7FF70C8DE2A0     (void* -> SkyrimSE.exe+2FEE2A0	pop rax)
	[RSP+6F0 ] 0x40000000         (size_t) [1073741824]
	[RSP+6F8 ] 0x0                (size_t) [0]
	[RSP+700 ] 0x0                (size_t) [0]
	[RSP+708 ] 0x1A2C2004B80      (TESQuest*)
		Active Quest: false
		Current Stage: 255
		Type: kCompanionsQuest
		File: "Unofficial Skyrim Special Edition Patch.esp"
		Modified by: Skyrim.esm -> Update.esm -> Unofficial Skyrim Special Edition Patch.esp
		Flags: 0x00400009 kDestructible | kInitialized
		Name: "Hired Muscle"
		EditorID: "CR04"
		FormID: 0x00025231
		FormType: Quest (77)
		GetFullName: "Hired Muscle"
	[RSP+710 ] 0x1                (size_t) [1]
	[RSP+718 ] 0x0                (size_t) [0]
	[RSP+720 ] 0x1A2C772A1B0      (BGSRefAlias*)
	[RSP+728 ] 0x8                (size_t) [8]
	[RSP+730 ] 0x4BF27FED89       (void*)
	[RSP+738 ] 0x7FF709C7D29D     (void* -> SkyrimSE.exe+038D29D	mov ecx, [rax])
	[RSP+740 ] 0x1A2C2004B80      (TESQuest*)
		Active Quest: false
		Current Stage: 255
		Type: kCompanionsQuest
		File: "Unofficial Skyrim Special Edition Patch.esp"
		Modified by: Skyrim.esm -> Update.esm -> Unofficial Skyrim Special Edition Patch.esp
		Flags: 0x00400009 kDestructible | kInitialized
		Name: "Hired Muscle"
		EditorID: "CR04"
		FormID: 0x00025231
		FormType: Quest (77)
		GetFullName: "Hired Muscle"
	[RSP+748 ] 0x4BF27FED58       (void*)
	[RSP+750 ] 0x1A2C772A101      (void*)
	[RSP+758 ] 0x2                (size_t) [2]
	[RSP+760 ] 0x4BF27FFC10       (void*)
	[RSP+768 ] 0x4BF27FEDF0       (void*)
	[RSP+770 ] 0x101C2AC3A01      (size_t) [1107072662017]
	[RSP+778 ] 0x1A22F3CE6D8      (char*) "o"
	[RSP+780 ] 0x1A300000005      (void*)
	[RSP+788 ] 0x7FF709C2CC8F     (void* -> SkyrimSE.exe+033CC8F	nop)
	[RSP+790 ] 0x1A3A1DB7740      (void*)
	[RSP+798 ] 0x1A2AA09C88B      (char*) "!"
	[RSP+7A0 ] 0x14               (size_t) [20]
	[RSP+7A8 ] 0x7FF70A38D4F5     (void* -> SkyrimSE.exe+0A9D4F5	mov r9, rax)
	[RSP+7B0 ] 0xFFFFFFFFFFFFFFFE (size_t) [uint: 18446744073709551614 int: -2]
	[RSP+7B8 ] 0x7FFD883657C3     (void* -> tbbmalloc.dll+00157C3	mov rbp, rax)
	[RSP+7C0 ] 0x14               (size_t) [20]
	[RSP+7C8 ] 0x1A2C2004C50      (void*)
	[RSP+7D0 ] 0x1A236AE8320      (BSTCommonLLMessageQueue<BSScript::Internal::FunctionMessage>*)
	[RSP+7D8 ] 0x7FFD00000000     (size_t) [140724603453440]
	[RSP+7E0 ] 0x1A236AE14E0      (void*)
	[RSP+7E8 ] 0x0                (size_t) [0]
	[RSP+7F0 ] 0x7FF70C8DA3A0     (void* -> SkyrimSE.exe+2FEA3A0	add [rax], al)
	[RSP+7F8 ] 0x7FF70AC4FBFD     (void* -> SkyrimSE.exe+135FBFD	mov eax, [rdi])
	[RSP+800 ] 0x1A22F3CDF70      (void*)
	[RSP+808 ] 0x1A3A1C1D14C      (void*)
	[RSP+810 ] 0xFFFFFFFFFFFFFFFE (size_t) [uint: 18446744073709551614 int: -2]
	[RSP+818 ] 0xCC6620F800000002 (size_t) [uint: 14728495880885764098 int: -3718248192823787518]
	[RSP+820 ] 0xFFFFFFFFFFFFFFFE (size_t) [uint: 18446744073709551614 int: -2]
	[RSP+828 ] 0x0                (size_t) [0]
	[RSP+830 ] 0x2                (size_t) [2]
	[RSP+838 ] 0xFFFFFFFF         (size_t) [4294967295]
	[RSP+840 ] 0x1A2C2AC3AC0      (BGSStoryManagerEventNode*)
		File: "HearthFires.esm"
		Modified by: Skyrim.esm -> HearthFires.esm
		Flags: 0x00000009 kDestructible | kInitialized
		EditorID: "Script Event"
		FormID: 0x0001379A
		FormType: StoryManagerEventNode (114)
	[RSP+848 ] 0x1A238398580      (BGSStoryManagerQuestFinder*)
	[RSP+850 ] 0x1A2C2AE3120      (BGSStoryManagerQuestNode*)
		File: "Skyrim.esm"
		Flags: 0x00000009 kDestructible | kInitialized
		FormID: 0x000BFC78
		FormType: StoryManagerQuestNode (113)
	[RSP+858 ] 0x2                (size_t) [2]
	[RSP+860 ] 0x1A2C2004B80      (TESQuest*)
		Active Quest: false
		Current Stage: 255
		Type: kCompanionsQuest
		File: "Unofficial Skyrim Special Edition Patch.esp"
		Modified by: Skyrim.esm -> Update.esm -> Unofficial Skyrim Special Edition Patch.esp
		Flags: 0x00400009 kDestructible | kInitialized
		Name: "Hired Muscle"
		EditorID: "CR04"
		FormID: 0x00025231
		FormType: Quest (77)
		GetFullName: "Hired Muscle"
	[RSP+868 ] 0x7FF709DDF95C     (void* -> SkyrimSE.exe+04EF95C	test al, al)
	[RSP+870 ] 0x0                (size_t) [0]
	[RSP+878 ] 0x1A39B9EBBA0      (char*) "W["
	[RSP+880 ] 0x4BF27FFC10       (void*)
	[RSP+888 ] 0x4BF27FEEA0       (void*)
	[RSP+890 ] 0x8                (size_t) [8]
	[RSP+898 ] 0x4BF27FF3B0       (void*)
	[RSP+8A0 ] 0x1A22F3CDF70      (void*)
	[RSP+8A8 ] 0x1A2A767C8E0      (void*)
	[RSP+8B0 ] 0xFFFFFFFFFFFFFFFE (size_t) [uint: 18446744073709551614 int: -2]
	[RSP+8B8 ] 0x1A22F3CE6D8      (char*) "o"
	[RSP+8C0 ] 0x1A3A287DEB4      (void*)
	[RSP+8C8 ] 0x1A2B3157040      (PlayerCharacter*)
		Flags: 0x00000408 
		Name: "Nadin"
		FormID: 0x00000014
		FormType: ActorCharacter (62)
		Flags: 0x00000408 
		Name: "Nadin"
		FormID: 0x00000014
		FormType: ActorCharacter (62)
		Object Reference: 
		File: "Skyrim.esm"
		Flags: 0x00040009 kDestructible | kInitialized
		Name: "Nadin"
		FormID: 0x00000007
		FormType: NPC (43)
		Flags: 0x00000408 kInitialized
		FormID: 0x00000014
		FormType: ActorCharacter (62)
	[RSP+8D0 ] 0x1A2B3157040      (PlayerCharacter*)
		Flags: 0x00000408 
		Name: "Nadin"
		FormID: 0x00000014
		FormType: ActorCharacter (62)
		Flags: 0x00000408 
		Name: "Nadin"
		FormID: 0x00000014
		FormType: ActorCharacter (62)
		Object Reference: 
		File: "Skyrim.esm"
		Flags: 0x00040009 kDestructible | kInitialized
		Name: "Nadin"
		FormID: 0x00000007
		FormType: NPC (43)
		Flags: 0x00000408 kInitialized
		FormID: 0x00000014
		FormType: ActorCharacter (62)
	[RSP+8D8 ] 0x0                (size_t) [0]
	[RSP+8E0 ] 0x1A39B9EBBA0      (char*) "W["
	[RSP+8E8 ] 0x0                (size_t) [0]
	[RSP+8F0 ] 0xFFFFFFFFFFFFFF00 (size_t) [uint: 18446744073709551360 int: -256]
	[RSP+8F8 ] 0x0                (size_t) [0]
	[RSP+900 ] 0x0                (size_t) [0]
	[RSP+908 ] 0x2                (size_t) [2]
	[RSP+910 ] 0x1A238398580      (BGSStoryManagerQuestFinder*)
	[RSP+918 ] 0x7FF709DDEFA3     (void* -> SkyrimSE.exe+04EEFA3	mov r14d, eax)
	[RSP+920 ] 0x1A203DAF200      (char*) "KILL"
	[RSP+928 ] 0x1A203DAF278      (char*) "SCPT"
	[RSP+930 ] 0x4BF27FEF69       (void*)
	[RSP+938 ] 0x1A2C2AE3120      (BGSStoryManagerQuestNode*)
		File: "Skyrim.esm"
		Flags: 0x00000009 kDestructible | kInitialized
		FormID: 0x000BFC78
		FormType: StoryManagerQuestNode (113)
	[RSP+940 ] 0x1A3966DBA00      (BSTriShape*)
		Name: "L1_FloraTundraCotton01:0 - L2_FloraTundraCotton01:0"
		RTTIName: "BSTriShape"
		Flags: kSelectiveUpdate | kSelectiveUpdateTransforms | kSelectiveUpdateController
		Full Name: "AlgodÃ£o da Tundra"
		File: "Plants\FloraTundraCotton01.nif"
		Checking User Data: -----
			Object Reference: 
			File: "Skyrim.esm"
			Flags: 0x00000009 kDestructible | kInitialized
			Name: "AlgodÃ£o da Tundra"
			FormID: 0x000BB947
			FormType: Tree (38)
		Checking TESObjectREFR: {}
			Object Reference: 
			File: "Skyrim.esm"
			Flags: 0x00000009 kDestructible | kInitialized
			Name: "AlgodÃ£o da Tundra"
			FormID: 0x000BB947
			FormType: Tree (38)
		Checking Parent: 1
			Name: "L1_FloraTundraCotton01"
			RTTIName: "NiNode"
			Flags: kSelectiveUpdate | kSelectiveUpdateTransforms | kSelectiveUpdateController
			Full Name: "AlgodÃ£o da Tundra"
			File: "Plants\FloraTundraCotton01.nif"
			Checking User Data: -----
				Object Reference: 
				File: "Skyrim.esm"
				Flags: 0x00000009 kDestructible | kInitialized
				Name: "AlgodÃ£o da Tundra"
				FormID: 0x000BB947
				FormType: Tree (38)
			Checking TESObjectREFR: {}
				Object Reference: 
				File: "Skyrim.esm"
				Flags: 0x00000009 kDestructible | kInitialized
				Name: "AlgodÃ£o da Tundra"
				FormID: 0x000BB947
				FormType: Tree (38)
			Checking Parent: 0
				Name: "FloraTundraCotton01"
				RTTIName: "BSLeafAnimNode"
				ExtraData[0] Name: "BSX"
				Flags: kSelectiveUpdate | kSelectiveUpdateTransforms | kSelectiveUpdateController
				Full Name: "AlgodÃ£o da Tundra"
				File: "Plants\FloraTundraCotton01.nif"
				Checking User Data: -----
					Object Reference: 
					File: "Skyrim.esm"
					Flags: 0x00000009 kDestructible | kInitialized
					Name: "AlgodÃ£o da Tundra"
					FormID: 0x000BB947
					FormType: Tree (38)
				Checking TESObjectREFR: {}
					Object Reference: 
					File: "Skyrim.esm"
					Flags: 0x00000009 kDestructible | kInitialized
					Name: "AlgodÃ£o da Tundra"
					FormID: 0x000BB947
					FormType: Tree (38)
				Checking Parent: 249
					RTTIName: "NiNode"
					Flags: kSelectiveUpdate | kSelectiveUpdateTransforms | kSelectiveUpdateController
					Checking Parent: 3
						RTTIName: "BSMultiBoundNode"
						Flags: kSelectiveUpdate | kSelectiveUpdateTransforms | kSelectiveUpdateController
						Checking Parent: 25
							Name: "ObjectLODRoot"
							RTTIName: "NiNode"
							Flags: kSelectiveUpdate | kSelectiveUpdateTransforms | kSelectiveUpdateController
							Checking Parent: 3
								Name: "shadow scene node"
								RTTIName: "ShadowSceneNode"
								Flags: kSelectiveUpdate | kSelectiveUpdateTransforms | kSelectiveUpdateController
								Checking Parent: 1
									Name: "WorldRoot Node"
									RTTIName: "SceneGraph"
									Flags: kSelectiveUpdate | kSelectiveUpdateTransforms | kSelectiveUpdateController
		Name: "L1_FloraTundraCotton01:0 - L2_FloraTundraCotton01:0"
	[RSP+948 ] 0x7FF70A69440F     (void* -> SkyrimSE.exe+0DA440F	nop)
	[RSP+950 ] 0x15               (size_t) [21]
	[RSP+958 ] 0x7FF70AC4FB7B     (void* -> SkyrimSE.exe+135FB7B	jmp 0x00007FF70AC4FB86)
	[RSP+960 ] 0xFFFFFFFF00000000 (size_t) [uint: 18446744069414584320 int: -4294967296]
	[RSP+968 ] 0x1A3A287DEB4      (void*)
	[RSP+970 ] 0xFFFFFFFFFFFFFFFE (size_t) [uint: 18446744073709551614 int: -2]
	[RSP+978 ] 0x7FF70AF0A598     (void* -> SkyrimSE.exe+161A598	nop)
	[RSP+980 ] 0xFFFFFFFFFFFFFFFE (size_t) [uint: 18446744073709551614 int: -2]
	[RSP+988 ] 0x7FF70AC93021     (void* -> SkyrimSE.exe+13A3021	nop)
	[RSP+990 ] 0x1A22F3CE6D8      (char*) "o"
	[RSP+998 ] 0x7FF70A59C998     (void* -> SkyrimSE.exe+0CAC998	nop)
	[RSP+9A0 ] 0x20               (size_t) [32]
	[RSP+9A8 ] 0xFFFFFFFF         (size_t) [4294967295]
	[RSP+9B0 ] 0xFFFFFFFF         (size_t) [4294967295]
	[RSP+9B8 ] 0x1A236EF1880      (BSGeometryListCullingProcess*)
	[RSP+9C0 ] 0x0                (size_t) [0]
	[RSP+9C8 ] 0x0                (size_t) [0]
	[RSP+9D0 ] 0x0                (size_t) [0]
	[RSP+9D8 ] 0x0                (size_t) [0]
	[RSP+9E0 ] 0x0                (size_t) [0]
	[RSP+9E8 ] 0x0                (size_t) [0]
	[RSP+9F0 ] 0x40000000         (size_t) [1073741824]
	[RSP+9F8 ] 0x0                (size_t) [0]
	[RSP+A00 ] 0xF0000003F        (size_t) [64424509503]
	[RSP+A08 ] 0x1A2C2B651E0      (BGSStoryManagerBranchNode*)
		File: "Skyrim.esm"
		Flags: 0x00000009 kDestructible | kInitialized
		FormID: 0x000F6085
		FormType: StoryManagerBranchNode (112)
	[RSP+A10 ] 0x7FF70C8B24B0     (BGSStoryManager*)
	[RSP+A18 ] 0x4BF27FFD00       (void*)
	[RSP+A20 ] 0x1A2C2AC3AC0      (BGSStoryManagerEventNode*)
		File: "HearthFires.esm"
		Modified by: Skyrim.esm -> HearthFires.esm
		Flags: 0x00000009 kDestructible | kInitialized
		EditorID: "Script Event"
		FormID: 0x0001379A
		FormType: StoryManagerEventNode (114)
	[RSP+A28 ] 0x1A238398580      (BGSStoryManagerQuestFinder*)
	[RSP+A30 ] 0x2                (size_t) [2]
	[RSP+A38 ] 0x1A203DAF278      (char*) "SCPT"
	[RSP+A40 ] 0x4BF27FF2E0       (void*)
	[RSP+A48 ] 0x7FF709DDECB6     (void* -> SkyrimSE.exe+04EECB6	mov esi, eax)
	[RSP+A50 ] 0x3CA101BC2C       (size_t) [260399283244]
	[RSP+A58 ] 0x300000034        (size_t) [12884901940]
	[RSP+A60 ] 0x300000001        (size_t) [12884901889]
	[RSP+A68 ] 0x3F00000002       (size_t) [270582939650]
	[RSP+A70 ] 0x3F00000003       (size_t) [270582939651]
	[RSP+A78 ] 0x3E00000003       (size_t) [266287972355]
	[RSP+A80 ] 0x3E00000003       (size_t) [266287972355]
	[RSP+A88 ] 0x1000000003       (size_t) [68719476739]
	[RSP+A90 ] 0xFFFFFFFFFFFFFFFE (size_t) [uint: 18446744073709551614 int: -2]
	[RSP+A98 ] 0x3C00000003       (size_t) [257698037763]
	[RSP+AA0 ] 0x1E00000003       (size_t) [128849018883]
	[RSP+AA8 ] 0x4B00000003       (size_t) [322122547203]
	[RSP+AB0 ] 0x4BF27FF189       (void*)
	[RSP+AB8 ] 0x7FF70A38FC4F     (void* -> SkyrimSE.exe+0A9FC4F	movzx eax, byte ptr [rsp+0x40])
	[RSP+AC0 ] 0x3F29E5C700000000 (size_t) [4551421541295849472]
	[RSP+AC8 ] 0x4B35800000       (size_t) [323020128256]
	[RSP+AD0 ] 0x1A2C2B64E20      (BGSStoryManagerBranchNode*)
		File: "Skyrim.esm"
		Flags: 0x00000009 kDestructible | kInitialized
		FormID: 0x000BFC76
		FormType: StoryManagerBranchNode (112)
	[RSP+AD8 ] 0x7FF70C8B24B0     (BGSStoryManager*)
	[RSP+AE0 ] 0x4BF27FFD00       (void*)
	[RSP+AE8 ] 0x1A2C2AC3AC0      (BGSStoryManagerEventNode*)
		File: "HearthFires.esm"
		Modified by: Skyrim.esm -> HearthFires.esm
		Flags: 0x00000009 kDestructible | kInitialized
		EditorID: "Script Event"
		FormID: 0x0001379A
		FormType: StoryManagerEventNode (114)
	[RSP+AF0 ] 0x1A238398580      (BGSStoryManagerQuestFinder*)
	[RSP+AF8 ] 0x7FF709DDECB6     (void* -> SkyrimSE.exe+04EECB6	mov esi, eax)
	[RSP+B00 ] 0x1A203DAF278      (char*) "SCPT"
	[RSP+B08 ] 0x4BF27FF2E0       (void*)
	[RSP+B10 ] 0x2                (size_t) [2]
	[RSP+B18 ] 0x7FF70A392D24     (void* -> SkyrimSE.exe+0AA2D24	mov rbx, [rsp+0x30])
	[RSP+B20 ] 0x1A22C6AF202      (void*)
	[RSP+B28 ] 0x7FF70A0171AF     (void* -> SkyrimSE.exe+07271AF	test al, al)
	[RSP+B30 ] 0x1A303AB7660      (void*)
	[RSP+B38 ] 0x6C61FC092F10B695 (size_t) [7809800345211680405]
	[RSP+B40 ] 0xFFFFFFFFFFFFFFFE (size_t) [uint: 18446744073709551614 int: -2]
	[RSP+B48 ] 0x7FF70A6F21C8     (void* -> SkyrimSE.exe+0E021C8	nop)
	[RSP+B50 ] 0x1A22C70EC20      (void*)
	[RSP+B58 ] 0x40               (size_t) [64]
	[RSP+B60 ] 0x30               (size_t) [48]
	[RSP+B68 ] 0x7FF70A52E93F     (void* -> SkyrimSE.exe+0C3E93F	cmp [rdi], eax)
	[RSP+B70 ] 0x0                (size_t) [0]
	[RSP+B78 ] 0x8000000000000000 (size_t) [uint: 9223372036854775808 int: -9223372036854775808]
	[RSP+B80 ] 0x1A2C2AC3AC0      (BGSStoryManagerEventNode*)
		File: "HearthFires.esm"
		Modified by: Skyrim.esm -> HearthFires.esm
		Flags: 0x00000009 kDestructible | kInitialized
		EditorID: "Script Event"
		FormID: 0x0001379A
		FormType: StoryManagerEventNode (114)
	[RSP+B88 ] 0x7FF70C8B24B0     (BGSStoryManager*)
	[RSP+B90 ] 0x4BF27FFD00       (void*)
	[RSP+B98 ] 0x1A2C2AC3AC0      (BGSStoryManagerEventNode*)
		File: "HearthFires.esm"
		Modified by: Skyrim.esm -> HearthFires.esm
		Flags: 0x00000009 kDestructible | kInitialized
		EditorID: "Script Event"
		FormID: 0x0001379A
		FormType: StoryManagerEventNode (114)
	[RSP+BA0 ] 0x1A238398580      (BGSStoryManagerQuestFinder*)
	[RSP+BA8 ] 0x7FF709DDECB6     (void* -> SkyrimSE.exe+04EECB6	mov esi, eax)
	[RSP+BB0 ] 0x1A203DAF278      (char*) "SCPT"
	[RSP+BB8 ] 0x4BF27FF2E0       (void*)
	[RSP+BC0 ] 0x2                (size_t) [2]
	[RSP+BC8 ] 0x1A22D095800      (ahkpWorld*)
	[RSP+BD0 ] 0x1A200000000      (void*)
	[RSP+BD8 ] 0x1A20D8B9300      (void*)
	[RSP+BE0 ] 0xC23F4D3641DB9740 (size_t) [uint: 13996991062319273792 int: -4449753011390277824]
	[RSP+BE8 ] 0xC1DB973F418E3926 (size_t) [uint: 13968924967158298918 int: -4477819106551252698]
	[RSP+BF0 ] 0xFFFFFFFFFFFFFFFE (size_t) [uint: 18446744073709551614 int: -2]
	[RSP+BF8 ] 0xC1DB973F418E3925 (size_t) [uint: 13968924967158298917 int: -4477819106551252699]
	[RSP+C00 ] 0x1A20705002B      (void*)
	[RSP+C08 ] 0x0                (size_t) [0]
	[RSP+C10 ] 0xFFFFFFFFFFFFFFFE (size_t) [uint: 18446744073709551614 int: -2]
	[RSP+C18 ] 0x1A22D095800      (ahkpWorld*)
	[RSP+C20 ] 0x0                (size_t) [0]
	[RSP+C28 ] 0x7FF70C8DCE60     (void* -> SkyrimSE.exe+2FECE60	rcl byte ptr [rdx+0x7FF70B0F], 0x00)
	[RSP+C30 ] 0x1A39B9EBBA0      (char*) "W["
	[RSP+C38 ] 0x7FF70C8B24B0     (BGSStoryManager*)
	[RSP+C40 ] 0x4BF27FFD00       (void*)
	[RSP+C48 ] 0x1A2C2AC3AC0      (BGSStoryManagerEventNode*)
		File: "HearthFires.esm"
		Modified by: Skyrim.esm -> HearthFires.esm
		Flags: 0x00000009 kDestructible | kInitialized
		EditorID: "Script Event"
		FormID: 0x0001379A
		FormType: StoryManagerEventNode (114)
	[RSP+C50 ] 0x0                (size_t) [0]
	[RSP+C58 ] 0x7FF709DDCB11     (void* -> SkyrimSE.exe+04ECB11	cmp eax, 0x01)
	[RSP+C60 ] 0x1A203DAF278      (char*) "SCPT"
	[RSP+C68 ] 0x4BF27FF2E0       (void*)
	[RSP+C70 ] 0xFFFFFFFFFFFFFFFF (size_t) [uint: 18446744073709551615 int: -1]
	[RSP+C78 ] 0xBDA43B94BDA43B94 (size_t) [uint: 13665112679371783060 int: -4781631394337768556]
	[RSP+C80 ] 0x0                (size_t) [0]
	[RSP+C88 ] 0x0                (size_t) [0]
	[RSP+C90 ] 0xFFFFFFFFFFFFFFFE (size_t) [uint: 18446744073709551614 int: -2]
	[RSP+C98 ] 0x1A2B3157040      (PlayerCharacter*)
		Flags: 0x00000408 
		Name: "Nadin"
		FormID: 0x00000014
		FormType: ActorCharacter (62)
		Flags: 0x00000408 
		Name: "Nadin"
		FormID: 0x00000014
		FormType: ActorCharacter (62)
		Object Reference: 
		File: "Skyrim.esm"
		Flags: 0x00040009 kDestructible | kInitialized
		Name: "Nadin"
		FormID: 0x00000007
		FormType: NPC (43)
		Flags: 0x00000408 kInitialized
		FormID: 0x00000014
		FormType: ActorCharacter (62)
	[RSP+CA0 ] 0x1A2B3157040      (PlayerCharacter*)
		Flags: 0x00000408 
		Name: "Nadin"
		FormID: 0x00000014
		FormType: ActorCharacter (62)
		Flags: 0x00000408 
		Name: "Nadin"
		FormID: 0x00000014
		FormType: ActorCharacter (62)
		Object Reference: 
		File: "Skyrim.esm"
		Flags: 0x00040009 kDestructible | kInitialized
		Name: "Nadin"
		FormID: 0x00000007
		FormType: NPC (43)
		Flags: 0x00000408 kInitialized
		FormID: 0x00000014
		FormType: ActorCharacter (62)
	[RSP+CA8 ] 0x0                (size_t) [0]
	[RSP+CB0 ] 0x1A39B9EBBA0      (char*) "W["
	[RSP+CB8 ] 0x0                (size_t) [0]
	[RSP+CC0 ] 0x4BF27FF300       (void*)
	[RSP+CC8 ] 0x0                (size_t) [0]
	[RSP+CD0 ] 0x0                (size_t) [0]
	[RSP+CD8 ] 0x0                (size_t) [0]
	[RSP+CE0 ] 0x0                (size_t) [0]
	[RSP+CE8 ] 0x0                (size_t) [0]
	[RSP+CF0 ] 0x0                (size_t) [0]
	[RSP+CF8 ] 0x0                (size_t) [0]
	[RSP+D00 ] 0x0                (size_t) [0]
	[RSP+D08 ] 0x0                (size_t) [0]
	[RSP+D10 ] 0x0                (size_t) [0]
	[RSP+D18 ] 0x0                (size_t) [0]
	[RSP+D20 ] 0x0                (size_t) [0]
	[RSP+D28 ] 0x0                (size_t) [0]
	[RSP+D30 ] 0x0                (size_t) [0]
	[RSP+D38 ] 0x0                (size_t) [0]
	[RSP+D40 ] 0x0                (size_t) [0]
	[RSP+D48 ] 0x0                (size_t) [0]
	[RSP+D50 ] 0x3F800000         (size_t) [1065353216]
	[RSP+D58 ] 0x0                (size_t) [0]
	[RSP+D60 ] 0x3F800000         (size_t) [1065353216]
	[RSP+D68 ] 0x0                (size_t) [0]
	[RSP+D70 ] 0xC604F90746B6F9AA (size_t) [uint: 14268803329063057834 int: -4177940744646493782]
	[RSP+D78 ] 0x7FF70A66F8A8     (void* -> SkyrimSE.exe+0D7F8A8	mov eax, [rbx+0x34])
	[RSP+D80 ] 0xC564C7F200000000 (size_t) [uint: 14223713365338882048 int: -4223030708370669568]
	[RSP+D88 ] 0xC625108D46B6F9AA (size_t) [uint: 14277836392610855338 int: -4168907681098696278]
	[RSP+D90 ] 0x46B6F9AAC55A40E6 (size_t) [5095534540267077862]
	[RSP+D98 ] 0xC564C7F2C625108D (size_t) [uint: 14223713368663199885 int: -4223030705046351731]
	[RSP+DA0 ] 0x1A39C06C580      (BSTriShape*)
		Name: "dm:0"
		RTTIName: "BSTriShape"
		Flags: kSelectiveUpdate | kSelectiveUpdateTransforms | kSelectiveUpdateController
		Full Name: "Dog Meat"
		File: "Clutter\Ingredients\DogMeat.nif"
		Checking Owner: -----
			File: "Skyrim.esm"
			Flags: 0x00000009 kDestructible | kInitialized
			Name: "FacÃ§Ã£o de ServiÃ§os de Whiterun - Anoriath"
			FormID: 0x00096F82
			FormType: Faction (11)
		Checking User Data: -----
			Object Reference: 
			File: "Unofficial Skyrim Special Edition Patch.esp"
			Modified by: Skyrim.esm -> ccQDRSSE001-SurvivalMode.esl -> Unofficial Skyrim Special Edition Patch.esp
			Flags: 0x00000009 kDestructible | kInitialized
			Name: "Dog Meat"
			FormID: 0x000EDB2E
			FormType: AlchemyItem (46)
		Checking TESObjectREFR: {}
			Object Reference: 
			File: "Unofficial Skyrim Special Edition Patch.esp"
			Modified by: Skyrim.esm -> ccQDRSSE001-SurvivalMode.esl -> Unofficial Skyrim Special Edition Patch.esp
			Flags: 0x00000009 kDestructible | kInitialized
			Name: "Dog Meat"
			FormID: 0x000EDB2E
			FormType: AlchemyItem (46)
		Checking Parent: 0
			Name: "dm"
			RTTIName: "BSFadeNode"
			ExtraData[0] Name: "INV"
			ExtraData[1] Name: "BSX"
			Flags: kSelectiveUpdate | kSelectiveUpdateTransforms | kSelectiveUpdateController
			Full Name: "Dog Meat"
			File: "Clutter\Ingredients\DogMeat.nif"
			Checking Owner: -----
				File: "Skyrim.esm"
				Flags: 0x00000009 kDestructible | kInitialized
				Name: "FacÃ§Ã£o de ServiÃ§os de Whiterun - Anoriath"
				FormID: 0x00096F82
				FormType: Faction (11)
			Checking User Data: -----
				Object Reference: 
				File: "Unofficial Skyrim Special Edition Patch.esp"
				Modified by: Skyrim.esm -> ccQDRSSE001-SurvivalMode.esl -> Unofficial Skyrim Special Edition Patch.esp
				Flags: 0x00000009 kDestructible | kInitialized
				Name: "Dog Meat"
				FormID: 0x000EDB2E
				FormType: AlchemyItem (46)
			Checking TESObjectREFR: {}
				Object Reference: 
				File: "Unofficial Skyrim Special Edition Patch.esp"
				Modified by: Skyrim.esm -> ccQDRSSE001-SurvivalMode.esl -> Unofficial Skyrim Special Edition Patch.esp
				Flags: 0x00000009 kDestructible | kInitialized
				Name: "Dog Meat"
				FormID: 0x000EDB2E
				FormType: AlchemyItem (46)
			Checking Parent: 297
				RTTIName: "NiNode"
				Flags: kSelectiveUpdate | kSelectiveUpdateTransforms | kSelectiveUpdateController
				Checking Parent: 3
					RTTIName: "BSMultiBoundNode"
					Flags: kSelectiveUpdate | kSelectiveUpdateTransforms | kSelectiveUpdateController
					Checking Parent: 25
						Name: "ObjectLODRoot"
						RTTIName: "NiNode"
						Flags: kSelectiveUpdate | kSelectiveUpdateTransforms | kSelectiveUpdateController
						Checking Parent: 3
							Name: "shadow scene node"
							RTTIName: "ShadowSceneNode"
							Flags: kSelectiveUpdate | kSelectiveUpdateTransforms | kSelectiveUpdateController
							Checking Parent: 1
								Name: "WorldRoot Node"
								RTTIName: "SceneGraph"
								Flags: kSelectiveUpdate | kSelectiveUpdateTransforms | kSelectiveUpdateController
		Name: "dm:0"
	[RSP+DA8 ] 0x7FF70A69440F     (void* -> SkyrimSE.exe+0DA440F	nop)
	[RSP+DB0 ] 0xC55300A8C6218CB8 (size_t) [uint: 14218709173417381048 int: -4228034900292170568]
	[RSP+DB8 ] 0xC61BEA4446BEBC81 (size_t) [uint: 14275261022846499969 int: -4171483050863051647]
	[RSP+DC0 ] 0x46BEBC81C5338EC0 (size_t) [5097719093775273664]
	[RSP+DC8 ] 0xC55300A8C61BEA44 (size_t) [uint: 14218709173417011780 int: -4228034900292539836]
	[RSP+DD0 ] 0xFFFFFFFFFFFFFFFE (size_t) [uint: 18446744073709551614 int: -2]
	[RSP+DD8 ] 0x7FF70AF0A598     (void* -> SkyrimSE.exe+161A598	nop)
	[RSP+DE0 ] 0x1A236EF19A8      (void*)
	[RSP+DE8 ] 0xC614600C46C312BD (size_t) [uint: 14273138724887007933 int: -4173605348822543683]
	[RSP+DF0 ] 0x1A22F3CE6D8      (char*) "o"
	[RSP+DF8 ] 0x7FF70A59C998     (void* -> SkyrimSE.exe+0CAC998	nop)
	[RSP+E00 ] 0x20               (size_t) [32]
	[RSP+E08 ] 0xFFFFFFFF         (size_t) [4294967295]
	[RSP+E10 ] 0xFFFFFFFF         (size_t) [4294967295]
	[RSP+E18 ] 0x1A236EF1880      (BSGeometryListCullingProcess*)
	[RSP+E20 ] 0xFFFFFFFFFFFFFFFE (size_t) [uint: 18446744073709551614 int: -2]
	[RSP+E28 ] 0x1A39BC67880      (NiNode*)
		Name: "L1_FloraTundraCotton01"
		RTTIName: "NiNode"
		Flags: kSelectiveUpdate | kSelectiveUpdateTransforms | kSelectiveUpdateController
		Full Name: "AlgodÃ£o da Tundra"
		File: "Plants\FloraTundraCotton01.nif"
		Checking User Data: -----
			Object Reference: 
			File: "Skyrim.esm"
			Flags: 0x00000009 kDestructible | kInitialized
			Name: "AlgodÃ£o da Tundra"
			FormID: 0x000BB947
			FormType: Tree (38)
		Checking TESObjectREFR: {}
			Object Reference: 
			File: "Skyrim.esm"
			Flags: 0x00000009 kDestructible | kInitialized
			Name: "AlgodÃ£o da Tundra"
			FormID: 0x000BB947
			FormType: Tree (38)
		Checking Parent: 0
			Name: "FloraTundraCotton01"
			RTTIName: "BSLeafAnimNode"
			ExtraData[0] Name: "BSX"
			Flags: kSelectiveUpdate | kSelectiveUpdateTransforms | kSelectiveUpdateController
			Full Name: "AlgodÃ£o da Tundra"
			File: "Plants\FloraTundraCotton01.nif"
			Checking User Data: -----
				Object Reference: 
				File: "Skyrim.esm"
				Flags: 0x00000009 kDestructible | kInitialized
				Name: "AlgodÃ£o da Tundra"
				FormID: 0x000BB947
				FormType: Tree (38)
			Checking TESObjectREFR: {}
				Object Reference: 
				File: "Skyrim.esm"
				Flags: 0x00000009 kDestructible | kInitialized
				Name: "AlgodÃ£o da Tundra"
				FormID: 0x000BB947
				FormType: Tree (38)
			Checking Parent: 249
				RTTIName: "NiNode"
				Flags: kSelectiveUpdate | kSelectiveUpdateTransforms | kSelectiveUpdateController
				Checking Parent: 3
					RTTIName: "BSMultiBoundNode"
					Flags: kSelectiveUpdate | kSelectiveUpdateTransforms | kSelectiveUpdateController
					Checking Parent: 25
						Name: "ObjectLODRoot"
						RTTIName: "NiNode"
						Flags: kSelectiveUpdate | kSelectiveUpdateTransforms | kSelectiveUpdateController
						Checking Parent: 3
							Name: "shadow scene node"
							RTTIName: "ShadowSceneNode"
							Flags: kSelectiveUpdate | kSelectiveUpdateTransforms | kSelectiveUpdateController
							Checking Parent: 1
								Name: "WorldRoot Node"
								RTTIName: "SceneGraph"
								Flags: kSelectiveUpdate | kSelectiveUpdateTransforms | kSelectiveUpdateController
		Name: "L1_FloraTundraCotton01"
	[RSP+E30 ] 0x1A236EF1880      (BSGeometryListCullingProcess*)
	[RSP+E38 ] 0x7FF70A68C421     (void* -> SkyrimSE.exe+0D9C421	mov [rdi+0x9C], r14d)
	[RSP+E40 ] 0x1A39BC6CA40      (BSMultiBoundNode*)
		RTTIName: "BSMultiBoundNode"
		Flags: kSelectiveUpdate | kSelectiveUpdateTransforms | kSelectiveUpdateController
		Full Name: ""
		File: "Architecture\WhiteRun\WRTerrain\WRWaterPool01.nif"
		Checking User Data: -----
			Object Reference: 
			File: "Update.esm"
			Modified by: Skyrim.esm -> Update.esm
			Flags: 0x00000009 kDestructible | kInitialized
			FormID: 0x00085FC9
			FormType: Activator (24)
		Checking TESObjectREFR: {}
			Object Reference: 
			File: "Update.esm"
			Modified by: Skyrim.esm -> Update.esm
			Flags: 0x00000009 kDestructible | kInitialized
			FormID: 0x00085FC9
			FormType: Activator (24)
		Checking Parent: 0
			Name: "WRWaterPool01"
			RTTIName: "BSFadeNode"
			ExtraData[0] Name: "BSX"
			Flags: kSelectiveUpdate | kSelectiveUpdateTransforms | kSelectiveUpdateController
			Full Name: ""
			File: "Architecture\WhiteRun\WRTerrain\WRWaterPool01.nif"
			Checking User Data: -----
				Object Reference: 
				File: "Update.esm"
				Modified by: Skyrim.esm -> Update.esm
				Flags: 0x00000009 kDestructible | kInitialized
				FormID: 0x00085FC9
				FormType: Activator (24)
			Checking TESObjectREFR: {}
				Object Reference: 
				File: "Update.esm"
				Modified by: Skyrim.esm -> Update.esm
				Flags: 0x00000009 kDestructible | kInitialized
				FormID: 0x00085FC9
				FormType: Activator (24)
			Checking Parent: 31
				RTTIName: "NiNode"
				Flags: kSelectiveUpdate | kSelectiveUpdateTransforms | kSelectiveUpdateController
				Checking Parent: 3
					RTTIName: "BSMultiBoundNode"
					Flags: kSelectiveUpdate | kSelectiveUpdateTransforms | kSelectiveUpdateController
					Checking Parent: 26
						Name: "ObjectLODRoot"
						RTTIName: "NiNode"
						Flags: kSelectiveUpdate | kSelectiveUpdateTransforms | kSelectiveUpdateController
						Checking Parent: 3
							Name: "shadow scene node"
							RTTIName: "ShadowSceneNode"
							Flags: kSelectiveUpdate | kSelectiveUpdateTransforms | kSelectiveUpdateController
							Checking Parent: 1
								Name: "WorldRoot Node"
								RTTIName: "SceneGraph"
								Flags: kSelectiveUpdate | kSelectiveUpdateTransforms | kSelectiveUpdateController
	[RSP+E48 ] 0x1A39C06C580      (BSTriShape*)
		Name: "dm:0"
		RTTIName: "BSTriShape"
		Flags: kSelectiveUpdate | kSelectiveUpdateTransforms | kSelectiveUpdateController
		Full Name: "Dog Meat"
		File: "Clutter\Ingredients\DogMeat.nif"
		Checking Owner: -----
			File: "Skyrim.esm"
			Flags: 0x00000009 kDestructible | kInitialized
			Name: "FacÃ§Ã£o de ServiÃ§os de Whiterun - Anoriath"
			FormID: 0x00096F82
			FormType: Faction (11)
		Checking User Data: -----
			Object Reference: 
			File: "Unofficial Skyrim Special Edition Patch.esp"
			Modified by: Skyrim.esm -> ccQDRSSE001-SurvivalMode.esl -> Unofficial Skyrim Special Edition Patch.esp
			Flags: 0x00000009 kDestructible | kInitialized
			Name: "Dog Meat"
			FormID: 0x000EDB2E
			FormType: AlchemyItem (46)
		Checking TESObjectREFR: {}
			Object Reference: 
			File: "Unofficial Skyrim Special Edition Patch.esp"
			Modified by: Skyrim.esm -> ccQDRSSE001-SurvivalMode.esl -> Unofficial Skyrim Special Edition Patch.esp
			Flags: 0x00000009 kDestructible | kInitialized
			Name: "Dog Meat"
			FormID: 0x000EDB2E
			FormType: AlchemyItem (46)
		Checking Parent: 0
			Name: "dm"
			RTTIName: "BSFadeNode"
			ExtraData[0] Name: "INV"
			ExtraData[1] Name: "BSX"
			Flags: kSelectiveUpdate | kSelectiveUpdateTransforms | kSelectiveUpdateController
			Full Name: "Dog Meat"
			File: "Clutter\Ingredients\DogMeat.nif"
			Checking Owner: -----
				File: "Skyrim.esm"
				Flags: 0x00000009 kDestructible | kInitialized
				Name: "FacÃ§Ã£o de ServiÃ§os de Whiterun - Anoriath"
				FormID: 0x00096F82
				FormType: Faction (11)
			Checking User Data: -----
				Object Reference: 
				File: "Unofficial Skyrim Special Edition Patch.esp"
				Modified by: Skyrim.esm -> ccQDRSSE001-SurvivalMode.esl -> Unofficial Skyrim Special Edition Patch.esp
				Flags: 0x00000009 kDestructible | kInitialized
				Name: "Dog Meat"
				FormID: 0x000EDB2E
				FormType: AlchemyItem (46)
			Checking TESObjectREFR: {}
				Object Reference: 
				File: "Unofficial Skyrim Special Edition Patch.esp"
				Modified by: Skyrim.esm -> ccQDRSSE001-SurvivalMode.esl -> Unofficial Skyrim Special Edition Patch.esp
				Flags: 0x00000009 kDestructible | kInitialized
				Name: "Dog Meat"
				FormID: 0x000EDB2E
				FormType: AlchemyItem (46)
			Checking Parent: 297
				RTTIName: "NiNode"
				Flags: kSelectiveUpdate | kSelectiveUpdateTransforms | kSelectiveUpdateController
				Checking Parent: 3
					RTTIName: "BSMultiBoundNode"
					Flags: kSelectiveUpdate | kSelectiveUpdateTransforms | kSelectiveUpdateController
					Checking Parent: 25
						Name: "ObjectLODRoot"
						RTTIName: "NiNode"
						Flags: kSelectiveUpdate | kSelectiveUpdateTransforms | kSelectiveUpdateController
						Checking Parent: 3
							Name: "shadow scene node"
							RTTIName: "ShadowSceneNode"
							Flags: kSelectiveUpdate | kSelectiveUpdateTransforms | kSelectiveUpdateController
							Checking Parent: 1
								Name: "WorldRoot Node"
								RTTIName: "SceneGraph"
								Flags: kSelectiveUpdate | kSelectiveUpdateTransforms | kSelectiveUpdateController
		Name: "dm:0"
	[RSP+E50 ] 0x1                (size_t) [1]
	[RSP+E58 ] 0xFFFFFFFF         (size_t) [4294967295]
	[RSP+E60 ] 0xF0000003F        (size_t) [64424509503]
	[RSP+E68 ] 0x2300000003       (size_t) [150323855363]
	[RSP+E70 ] 0x3F00000003       (size_t) [270582939651]
	[RSP+E78 ] 0x2F00000003       (size_t) [201863462915]
	[RSP+E80 ] 0x3F00000003       (size_t) [270582939651]
	[RSP+E88 ] 0x3F00000003       (size_t) [270582939651]
	[RSP+E90 ] 0x3F00000003       (size_t) [270582939651]
	[RSP+E98 ] 0x3F00000003       (size_t) [270582939651]
	[RSP+EA0 ] 0x1F00000003       (size_t) [133143986179]
	[RSP+EA8 ] 0xE00000003        (size_t) [60129542147]
	[RSP+EB0 ] 0x3D00000003       (size_t) [261993005059]
	[RSP+EB8 ] 0x300000035        (size_t) [12884901941]
	[RSP+EC0 ] 0x30000003F        (size_t) [12884901951]
	[RSP+EC8 ] 0x3F0000003D       (size_t) [270582939709]
	[RSP+ED0 ] 0x3F00000003       (size_t) [270582939651]
	[RSP+ED8 ] 0x3F00000003       (size_t) [270582939651]
	[RSP+EE0 ] 0x3F00000003       (size_t) [270582939651]
	[RSP+EE8 ] 0x1F00000003       (size_t) [133143986179]
	[RSP+EF0 ] 0x3F00000000       (size_t) [270582939648]
	[RSP+EF8 ] 0x3F00000003       (size_t) [270582939651]
	[RSP+F00 ] 0x1F00000003       (size_t) [133143986179]
	[RSP+F08 ] 0x7FF700000003     (size_t) [140698833649667]
	[RSP+F10 ] 0x5                (size_t) [5]
	[RSP+F18 ] 0x0                (size_t) [0]
	[RSP+F20 ] 0x2                (size_t) [2]
	[RSP+F28 ] 0x0                (size_t) [0]
	[RSP+F30 ] 0x5                (size_t) [5]
	[RSP+F38 ] 0x0                (size_t) [0]
	[RSP+F40 ] 0x0                (size_t) [0]
	[RSP+F48 ] 0x7FF70A41C4C2     (void* -> SkyrimSE.exe+0B2C4C2	test rax, rax)
	[RSP+F50 ] 0x4BF27FF8F8       (char*) "5"
	[RSP+F58 ] 0x7FFDCDDE8848     (void* -> ucrtbase.dll+0038848	movaps xmm0, xmm6)
	[RSP+F60 ] 0x1A3A1A8F800      (void*)
	[RSP+F68 ] 0x17               (size_t) [23]
	[RSP+F70 ] 0xBBADC3E2BBA57B49 (size_t) [uint: 13523680634641677129 int: -4923063439067874487]
	[RSP+F78 ] 0x7FF709DFE59E     (void* -> SkyrimSE.exe+050E59E	test al, al)
	[RSP+F80 ] 0x3C257A24BC2DC2AE (size_t) [4334004514608497326]
	[RSP+F88 ] 0xBE4FAD363F7FF900 (size_t) [uint: 13713369838871640320 int: -4733374234837911296]
	[RSP+F90 ] 0xFFFFFFFFFFFFFFFE (size_t) [uint: 18446744073709551614 int: -2]
	[RSP+F98 ] 0x3FD189B2C553B5C3 (size_t) [4598608095429768643]
	[RSP+FA0 ] 0x1A39283AD40      (BSAnimationGraphManager*)
	[RSP+FA8 ] 0x7FF709F3B48B     (void* -> SkyrimSE.exe+064B48B	cmp [rbx], eax)
	[RSP+FB0 ] 0x80000000         (size_t) [2147483648]
	[RSP+FB8 ] 0x0                (size_t) [0]
	[RSP+FC0 ] 0x0                (size_t) [0]
	[RSP+FC8 ] 0x4BF27FF750       (void*)
	[RSP+FD0 ] 0xFFFFFFFFFFFFFFFE (size_t) [uint: 18446744073709551614 int: -2]
	[RSP+FD8 ] 0x7FF709F0B381     (void* -> SkyrimSE.exe+061B381	test al, al)
	[RSP+FE0 ] 0x4BF27FF8F8       (char*) "5"
	[RSP+FE8 ] 0x1A3A1BD8800      (bhkCharRigidBodyController*)
	[RSP+FF0 ] 0x1A2BA9B3700      (Character*)
		File: "Skyrim.esm"
		Flags: 0x00400449 
		Name: "Eorlund Gray-Mane"
		FormID: 0x0001A683
		FormType: ActorCharacter (62)
		Object Reference: 
		File: "Immersive Weapons.esp"
		Modified by: Skyrim.esm -> Unofficial Skyrim Special Edition Patch.esp -> Immersive Weapons.esp
		Flags: 0x00440009 kDestructible | kInitialized
		Name: "Eorlund Gray-Mane"
		FormID: 0x00013B9D
		FormType: NPC (43)
		File: "Skyrim.esm"
		Flags: 0x00400449 kDestructible | kInitialized | kBorderRegion
		FormID: 0x0001A683
		FormType: ActorCharacter (62)
	[RSP+FF8 ] 0x4BF27FF690       (void*)
	[RSP+1000] 0x1A2BA9B37D0      (Character*)
		File: "Skyrim.esm"
		Flags: 0x00400449 
		Name: "Eorlund Gray-Mane"
		FormID: 0x0001A683
		FormType: ActorCharacter (62)
		Object Reference: 
		File: "Immersive Weapons.esp"
		Modified by: Skyrim.esm -> Unofficial Skyrim Special Edition Patch.esp -> Immersive Weapons.esp
		Flags: 0x00440009 kDestructible | kInitialized
		Name: "Eorlund Gray-Mane"
		FormID: 0x00013B9D
		FormType: NPC (43)
		File: "Skyrim.esm"
		Flags: 0x00400449 kDestructible | kInitialized | kBorderRegion
		FormID: 0x0001A683
		FormType: ActorCharacter (62)
	[RSP+1008] 0x7FF709F3543D     (void* -> SkyrimSE.exe+064543D	test al, al)
	[RSP+1010] 0x1A20000003A      (void*)
	[RSP+1018] 0x4BF27FF690       (void*)
	[RSP+1020] 0x1A39283AD40      (BSAnimationGraphManager*)
	[RSP+1028] 0x1A39283ADE0      (void*)
	[RSP+1030] 0xBF0A6CA73F57590A (size_t) [uint: 13765934676589369610 int: -4680809397120182006]
	[RSP+1038] 0x3F0A6CA700000000 (size_t) [4542562638671904768]
	[RSP+1040] 0x3F57590A         (size_t) [1062689034]
	[RSP+1048] 0x0                (size_t) [0]
	[RSP+1050] 0x1A33F800000      (void*)
	[RSP+1058] 0x8000000080000000 (size_t) [uint: 9223372039002259456 int: -9223372034707292160]
	[RSP+1060] 0x3AB40ED7         (size_t) [984878807]
	[RSP+1068] 0x0                (size_t) [0]
	[RSP+1070] 0x3F722276         (size_t) [1064444534]
	[RSP+1078] 0xBC32C44EBD771170 (size_t) [uint: 13561117270431175024 int: -4885626803278376592]
	[RSP+1080] 0x3FABD000         (size_t) [1068224512]
	[RSP+1088] 0x7FF70A2F04BE     (void* -> SkyrimSE.exe+0A004BE	mulss xmm0, xmm8)
	[RSP+1090] 0x3CDDD8A0         (size_t) [1021171872]
	[RSP+1098] 0x3E280000         (size_t) [1042808832]
	[RSP+10A0] 0x0                (size_t) [0]
	[RSP+10A8] 0x0                (size_t) [0]
	[RSP+10B0] 0x0                (size_t) [0]
	[RSP+10B8] 0x0                (size_t) [0]
	[RSP+10C0] 0x0                (size_t) [0]
	[RSP+10C8] 0x0                (size_t) [0]
	[RSP+10D0] 0x3F800000         (size_t) [1065353216]
	[RSP+10D8] 0x0                (size_t) [0]
	[RSP+10E0] 0x3E12A8C8         (size_t) [1041410248]
	[RSP+10E8] 0x0                (size_t) [0]
	[RSP+10F0] 0x3F060A92         (size_t) [1057360530]
	[RSP+10F8] 0x0                (size_t) [0]
	[RSP+1100] 0x4BF27FF6F0       (void*)
	[RSP+1108] 0xFFFFFFFFFFFFFFFE (size_t) [uint: 18446744073709551614 int: -2]
	[RSP+1110] 0x0                (size_t) [0]
	[RSP+1118] 0x1A22CBC8A20      (hkbFootIkDriver*)
	[RSP+1120] 0x3F7FFFF0         (size_t) [1065353200]
	[RSP+1128] 0x0                (size_t) [0]
	[RSP+1130] 0x3AB415003F7FFFF0 (size_t) [4230029040817274864]
	[RSP+1138] 0xBAB4150000000000 (size_t) [uint: 13453401076606697472 int: -4993342997102854144]
	[RSP+1140] 0x0                (size_t) [0]
	[RSP+1148] 0x0                (size_t) [0]
	[RSP+1150] 0xBAB41500         (size_t) [3132364032]
	[RSP+1158] 0x0                (size_t) [0]
	[RSP+1160] 0x3F7FFFF0         (size_t) [1065353200]
	[RSP+1168] 0x0                (size_t) [0]
	[RSP+1170] 0x3AB41500         (size_t) [984880384]
	[RSP+1178] 0x0                (size_t) [0]
	[RSP+1180] 0x3F800000         (size_t) [1065353216]
	[RSP+1188] 0x0                (size_t) [0]
	[RSP+1190] 0x3F800000         (size_t) [1065353216]
	[RSP+1198] 0x0                (size_t) [0]
	[RSP+11A0] 0x4BF27FF8F8       (char*) "5"
	[RSP+11A8] 0x1A2CEF50910      (void*)
	[RSP+11B0] 0x1A39BBE3948      (char*) "(2411704D)"
	[RSP+11B8] 0x1A39BBE3940      (void*)
	[RSP+11C0] 0x4BF27FF8E0       (void*)
	[RSP+11C8] 0x7FF70ACA46F0     (void* -> SkyrimSE.exe+13B46F0	lea rcx, [0x00007FF70CB5B238])
	[RSP+11D0] 0x1                (size_t) [1]
	[RSP+11D8] 0x1A22F3CDF70      (void*)
	[RSP+11E0] 0x4BF27FF8E0       (void*)
	[RSP+11E8] 0x0                (size_t) [0]
	[RSP+11F0] 0x0                (size_t) [0]
	[RSP+11F8] 0x0                (size_t) [0]
	[RSP+1200] 0x0                (size_t) [0]
	[RSP+1208] 0x0                (size_t) [0]
	[RSP+1210] 0x3F800000         (size_t) [1065353216]
	[RSP+1218] 0x0                (size_t) [0]
	[RSP+1220] 0x3F800000         (size_t) [1065353216]
	[RSP+1228] 0x0                (size_t) [0]
	[RSP+1230] 0x1A39665FA00      (BSLeafAnimNode*)
		Name: "DeadShrub01"
		RTTIName: "BSLeafAnimNode"
		Flags: kSelectiveUpdate | kSelectiveUpdateTransforms | kSelectiveUpdateController
		Full Name: ""
		File: "Landscape\Plants\DeadShrub01.nif"
		Checking User Data: -----
			Object Reference: 
			File: "Skyrim.esm"
			Flags: 0x00000009 kDestructible | kInitialized
			FormID: 0x000A731C
			FormType: Tree (38)
		Checking TESObjectREFR: {}
			Object Reference: 
			File: "Skyrim.esm"
			Flags: 0x00000009 kDestructible | kInitialized
			FormID: 0x000A731C
			FormType: Tree (38)
		Checking Parent: 277
			RTTIName: "NiNode"
			Flags: kSelectiveUpdate | kSelectiveUpdateTransforms | kSelectiveUpdateController
			Checking Parent: 3
				RTTIName: "BSMultiBoundNode"
				Flags: kSelectiveUpdate | kSelectiveUpdateTransforms | kSelectiveUpdateController
				Checking Parent: 25
					Name: "ObjectLODRoot"
					RTTIName: "NiNode"
					Flags: kSelectiveUpdate | kSelectiveUpdateTransforms | kSelectiveUpdateController
					Checking Parent: 3
						Name: "shadow scene node"
						RTTIName: "ShadowSceneNode"
						Flags: kSelectiveUpdate | kSelectiveUpdateTransforms | kSelectiveUpdateController
						Checking Parent: 1
							Name: "WorldRoot Node"
							RTTIName: "SceneGraph"
							Flags: kSelectiveUpdate | kSelectiveUpdateTransforms | kSelectiveUpdateController
		Name: "DeadShrub01"
	[RSP+1238] 0x7FF70ACA438C     (void* -> SkyrimSE.exe+13B438C	mov eax, [rbx+0xF4])
	[RSP+1240] 0x1A236EF1800      (void*)
	[RSP+1248] 0x7FF70ACA46F0     (void* -> SkyrimSE.exe+13B46F0	lea rcx, [0x00007FF70CB5B238])
	[RSP+1250] 0x4BF27FF8E0       (void*)
	[RSP+1258] 0x7FF70A414B4E     (void* -> SkyrimSE.exe+0B24B4E	lea r11, [rsp+0x208])
	[RSP+1260] 0x1                (size_t) [1]
	[RSP+1268] 0x7FF70A582D3B     (void* -> SkyrimSE.exe+0C92D3B	add rbx, 0x08)
	[RSP+1270] 0xFFFFFFFF         (size_t) [4294967295]
	[RSP+1278] 0x1A236EF1880      (BSGeometryListCullingProcess*)
	[RSP+1280] 0x0                (size_t) [0]
	[RSP+1288] 0x1A3966CDA80      (BSFadeNode*)
		Name: "WRWaterPool01"
		RTTIName: "BSFadeNode"
		ExtraData[0] Name: "BSX"
		Flags: kSelectiveUpdate | kSelectiveUpdateTransforms | kSelectiveUpdateController
		Full Name: ""
		File: "Architecture\WhiteRun\WRTerrain\WRWaterPool01.nif"
		Checking User Data: -----
			Object Reference: 
			File: "Update.esm"
			Modified by: Skyrim.esm -> Update.esm
			Flags: 0x00000009 kDestructible | kInitialized
			FormID: 0x00085FC9
			FormType: Activator (24)
		Checking TESObjectREFR: {}
			Object Reference: 
			File: "Update.esm"
			Modified by: Skyrim.esm -> Update.esm
			Flags: 0x00000009 kDestructible | kInitialized
			FormID: 0x00085FC9
			FormType: Activator (24)
		Checking Parent: 31
			RTTIName: "NiNode"
			Flags: kSelectiveUpdate | kSelectiveUpdateTransforms | kSelectiveUpdateController
			Checking Parent: 3
				RTTIName: "BSMultiBoundNode"
				Flags: kSelectiveUpdate | kSelectiveUpdateTransforms | kSelectiveUpdateController
				Checking Parent: 26
					Name: "ObjectLODRoot"
					RTTIName: "NiNode"
					Flags: kSelectiveUpdate | kSelectiveUpdateTransforms | kSelectiveUpdateController
					Checking Parent: 3
						Name: "shadow scene node"
						RTTIName: "ShadowSceneNode"
						Flags: kSelectiveUpdate | kSelectiveUpdateTransforms | kSelectiveUpdateController
						Checking Parent: 1
							Name: "WorldRoot Node"
							RTTIName: "SceneGraph"
							Flags: kSelectiveUpdate | kSelectiveUpdateTransforms | kSelectiveUpdateController
		Name: "WRWaterPool01"
	[RSP+1290] 0x1A236EF1880      (BSGeometryListCullingProcess*)
	[RSP+1298] 0x7FF70ACA4326     (void* -> SkyrimSE.exe+13B4326	mov rbx, [rsp+0x60])
	[RSP+12A0] 0x1A3966CDA80      (BSFadeNode*)
		Name: "WRWaterPool01"
		RTTIName: "BSFadeNode"
		ExtraData[0] Name: "BSX"
		Flags: kSelectiveUpdate | kSelectiveUpdateTransforms | kSelectiveUpdateController
		Full Name: ""
		File: "Architecture\WhiteRun\WRTerrain\WRWaterPool01.nif"
		Checking User Data: -----
			Object Reference: 
			File: "Update.esm"
			Modified by: Skyrim.esm -> Update.esm
			Flags: 0x00000009 kDestructible | kInitialized
			FormID: 0x00085FC9
			FormType: Activator (24)
		Checking TESObjectREFR: {}
			Object Reference: 
			File: "Update.esm"
			Modified by: Skyrim.esm -> Update.esm
			Flags: 0x00000009 kDestructible | kInitialized
			FormID: 0x00085FC9
			FormType: Activator (24)
		Checking Parent: 31
			RTTIName: "NiNode"
			Flags: kSelectiveUpdate | kSelectiveUpdateTransforms | kSelectiveUpdateController
			Checking Parent: 3
				RTTIName: "BSMultiBoundNode"
				Flags: kSelectiveUpdate | kSelectiveUpdateTransforms | kSelectiveUpdateController
				Checking Parent: 26
					Name: "ObjectLODRoot"
					RTTIName: "NiNode"
					Flags: kSelectiveUpdate | kSelectiveUpdateTransforms | kSelectiveUpdateController
					Checking Parent: 3
						Name: "shadow scene node"
						RTTIName: "ShadowSceneNode"
						Flags: kSelectiveUpdate | kSelectiveUpdateTransforms | kSelectiveUpdateController
						Checking Parent: 1
							Name: "WorldRoot Node"
							RTTIName: "SceneGraph"
							Flags: kSelectiveUpdate | kSelectiveUpdateTransforms | kSelectiveUpdateController
		Name: "WRWaterPool01"
	[RSP+12A8] 0x1A236EF1880      (BSGeometryListCullingProcess*)
	[RSP+12B0] 0x1                (size_t) [1]
	[RSP+12B8] 0xFFFFFFFF         (size_t) [4294967295]
	[RSP+12C0] 0xC5E7FCEB469D06B3 (size_t) [uint: 14260644832524175027 int: -4186099241185376589]
	[RSP+12C8] 0x3F800000C559DD3D (size_t) [4575657224719424829]
	[RSP+12D0] 0x0                (size_t) [0]
	[RSP+12D8] 0x0                (size_t) [0]
	[RSP+12E0] 0x0                (size_t) [0]
	[RSP+12E8] 0x0                (size_t) [0]
	[RSP+12F0] 0x1A236EF1880      (BSGeometryListCullingProcess*)
	[RSP+12F8] 0x7FF70A68C421     (void* -> SkyrimSE.exe+0D9C421	mov [rdi+0x9C], r14d)
	[RSP+1300] 0x1A396421480      (BSFadeNode*)
		Name: "FXSplashSmallParticlesLong"
		RTTIName: "BSFadeNode"
		ExtraData[0] Name: "BSX"
		Flags: kSelectiveUpdate | kSelectiveUpdateTransforms | kSelectiveUpdateController
		Full Name: ""
		File: "Effects\FXSplashSmallParticlesLong.nif"
		Checking User Data: -----
			Object Reference: 
			File: "Skyrim.esm"
			Flags: 0x00010009 kDestructible | kInitialized
			FormID: 0x0002BCA7
			FormType: MovableStatic (36)
		Checking TESObjectREFR: {}
			Object Reference: 
			File: "Skyrim.esm"
			Flags: 0x00010009 kDestructible | kInitialized
			FormID: 0x0002BCA7
			FormType: MovableStatic (36)
		Checking Parent: 121
			RTTIName: "NiNode"
			Flags: kSelectiveUpdate | kSelectiveUpdateTransforms | kSelectiveUpdateController
			Checking Parent: 3
				RTTIName: "BSMultiBoundNode"
				Flags: kSelectiveUpdate | kSelectiveUpdateTransforms | kSelectiveUpdateController
				Checking Parent: 27
					Name: "ObjectLODRoot"
					RTTIName: "NiNode"
					Flags: kSelectiveUpdate | kSelectiveUpdateTransforms | kSelectiveUpdateController
					Checking Parent: 3
						Name: "shadow scene node"
						RTTIName: "ShadowSceneNode"
						Flags: kSelectiveUpdate | kSelectiveUpdateTransforms | kSelectiveUpdateController
						Checking Parent: 1
							Name: "WorldRoot Node"
							RTTIName: "SceneGraph"
							Flags: kSelectiveUpdate | kSelectiveUpdateTransforms | kSelectiveUpdateController
		Name: "FXSplashSmallParticlesLong"
	[RSP+1308] 0xFFFFFFFF         (size_t) [4294967295]
	[RSP+1310] 0x3F               (size_t) [63]
	[RSP+1318] 0x45D0DF3C         (size_t) [1171316540]
	[RSP+1320] 0xF0000003F        (size_t) [64424509503]
	[RSP+1328] 0x2300000003       (size_t) [150323855363]
	[RSP+1330] 0x3F00000003       (size_t) [270582939651]
	[RSP+1338] 0x2F00000003       (size_t) [201863462915]
	[RSP+1340] 0x3F00000003       (size_t) [270582939651]
	[RSP+1348] 0x3F00000003       (size_t) [270582939651]
	[RSP+1350] 0x3F00000003       (size_t) [270582939651]
	[RSP+1358] 0x3F00000003       (size_t) [270582939651]
	[RSP+1360] 0x1F00000003       (size_t) [133143986179]
	[RSP+1368] 0xE00000003        (size_t) [60129542147]
	[RSP+1370] 0x3D00000003       (size_t) [261993005059]
	[RSP+1378] 0x300000035        (size_t) [12884901941]
	[RSP+1380] 0x30000003F        (size_t) [12884901951]
	[RSP+1388] 0x3F0000003D       (size_t) [270582939709]
	[RSP+1390] 0x3F00000003       (size_t) [270582939651]
	[RSP+1398] 0x3F00000003       (size_t) [270582939651]
	[RSP+13A0] 0x3F00000003       (size_t) [270582939651]
	[RSP+13A8] 0x1F00000003       (size_t) [133143986179]
	[RSP+13B0] 0x3F00000000       (size_t) [270582939648]
	[RSP+13B8] 0x3F00000003       (size_t) [270582939651]
	[RSP+13C0] 0x1F00000003       (size_t) [133143986179]
	[RSP+13C8] 0x3                (size_t) [3]
	[RSP+13D0] 0x0                (size_t) [0]
	[RSP+13D8] 0x0                (size_t) [0]
	[RSP+13E0] 0x0                (size_t) [0]
	[RSP+13E8] 0x0                (size_t) [0]
	[RSP+13F0] 0x0                (size_t) [0]
	[RSP+13F8] 0x0                (size_t) [0]
	[RSP+1400] 0x0                (size_t) [0]
	[RSP+1408] 0x0                (size_t) [0]
	[RSP+1410] 0x0                (size_t) [0]
	[RSP+1418] 0x0                (size_t) [0]
	[RSP+1420] 0x0                (size_t) [0]
	[RSP+1428] 0x0                (size_t) [0]
	[RSP+1430] 0x3C89E60F         (size_t) [1015670287]
	[RSP+1438] 0x0                (size_t) [0]
	[RSP+1440] 0x3C89E60F         (size_t) [1015670287]
	[RSP+1448] 0x0                (size_t) [0]
	[RSP+1450] 0x32               (size_t) [50]
	[RSP+1458] 0x1A2CEF50900      (BShkbAnimationGraph*)
		Project Name: "DefaultMale"
		Holder: 
			Object Reference: 
			File: "Immersive Weapons.esp"
			Modified by: Skyrim.esm -> Unofficial Skyrim Special Edition Patch.esp -> Immersive Weapons.esp
			Flags: 0x00440009 kDestructible | kInitialized
			Name: "Eorlund Gray-Mane"
			FormID: 0x00013B9D
			FormType: NPC (43)
	[RSP+1460] 0x3A               (size_t) [58]
	[RSP+1468] 0x1A2CEF50900      (BShkbAnimationGraph*)
		Project Name: "DefaultMale"
		Holder: 
			Object Reference: 
			File: "Immersive Weapons.esp"
			Modified by: Skyrim.esm -> Unofficial Skyrim Special Edition Patch.esp -> Immersive Weapons.esp
			Flags: 0x00440009 kDestructible | kInitialized
			Name: "Eorlund Gray-Mane"
			FormID: 0x00013B9D
			FormType: NPC (43)
	[RSP+1470] 0x4BF27FFB00       (void*)
	[RSP+1478] 0x7FF70A415B63     (void* -> SkyrimSE.exe+0B25B63	lea r11, [rsp+0x110])
	[RSP+1480] 0x1A3BF0A6CA7      (void*)
	[RSP+1488] 0x3F57590A         (size_t) [1062689034]
	[RSP+1490] 0x4B80000000       (size_t) [324270030848]
	[RSP+1498] 0x3F57590A         (size_t) [1062689034]
	[RSP+14A0] 0x0                (size_t) [0]
	[RSP+14A8] 0x7FFD883657C3     (void* -> tbbmalloc.dll+00157C3	mov rbp, rax)
	[RSP+14B0] 0x1A3E10F6040      (void*)
	[RSP+14B8] 0x7FFD883657C3     (void* -> tbbmalloc.dll+00157C3	mov rbp, rax)
	[RSP+14C0] 0x0                (size_t) [0]
	[RSP+14C8] 0xFFFFFF00         (size_t) [4294967040]
	[RSP+14D0] 0x1A22D095800      (ahkpWorld*)
	[RSP+14D8] 0x800000000        (size_t) [34359738368]
	[RSP+14E0] 0xC597800046B28000 (size_t) [uint: 14237989485629571072 int: -4208754588079980544]
	[RSP+14E8] 0xC539981B         (size_t) [3308886043]
	[RSP+14F0] 0x0                (size_t) [0]
	[RSP+14F8] 0x3F7593C2BE909B95 (size_t) [4572723461294693269]
	[RSP+1500] 0x3F83D70A3F83D70A (size_t) [4576738085353805578]
	[RSP+1508] 0x3F83D70A3F83D70A (size_t) [4576738085353805578]
	[RSP+1510] 0xFFFFFFFFFFFFFFFE (size_t) [uint: 18446744073709551614 int: -2]
	[RSP+1518] 0x7FF70AA55454     (void* -> SkyrimSE.exe+1165454	ucomiss xmm7, xmm6)
	[RSP+1520] 0xFFFFFFFFFFFFFFFE (size_t) [uint: 18446744073709551614 int: -2]
	[RSP+1528] 0x0                (size_t) [0]
	[RSP+1530] 0x4BF27FFB10       (void*)
	[RSP+1538] 0x7FF70C982644     (void* -> SkyrimSE.exe+3092644	add [rax], al)
	[RSP+1540] 0x1                (size_t) [1]
	[RSP+1548] 0x8                (size_t) [8]
	[RSP+1550] 0x8                (size_t) [8]
	[RSP+1558] 0x1                (size_t) [1]
	[RSP+1560] 0x7FFD883883C0     (void* -> tbbmalloc.dll+00383C0	add [rax], al)
	[RSP+1568] 0x7FFD88367A16     (void* -> tbbmalloc.dll+0017A16	mov rsi, rax)
	[RSP+1570] 0x3C89E60F         (size_t) [1015670287]
	[RSP+1578] 0x0                (size_t) [0]
	[RSP+1580] 0x3C89E60F         (size_t) [1015670287]
	[RSP+1588] 0x7FF70A413C8E     (void* -> SkyrimSE.exe+0B23C8E	mov rax, [rax+0x10])
	[RSP+1590] 0x0                (size_t) [0]
	[RSP+1598] 0x1A22F3CDF70      (void*)
	[RSP+15A0] 0x4BF27FFCB8       (void*)
	[RSP+15A8] 0xFFFFFFFFFFFFFFFE (size_t) [uint: 18446744073709551614 int: -2]
	[RSP+15B0] 0x4BF27FFBE0       (void*)
	[RSP+15B8] 0x8                (size_t) [8]
	[RSP+15C0] 0xFFFFFFFF         (size_t) [4294967295]
	[RSP+15C8] 0x1A22F3CDF70      (void*)
	[RSP+15D0] 0x1                (size_t) [1]
	[RSP+15D8] 0x1                (size_t) [1]
	[RSP+15E0] 0x7FF70C982644     (void* -> SkyrimSE.exe+3092644	add [rax], al)
	[RSP+15E8] 0x1                (size_t) [1]
	[RSP+15F0] 0xFFFFFFFF         (size_t) [4294967295]
	[RSP+15F8] 0x1A22F3CDF70      (void*)
	[RSP+1600] 0x7FF70C8B23D0     (BGSStoryTeller*)
	[RSP+1608] 0x0                (size_t) [0]
	[RSP+1610] 0x4BF27FFCA0       (void*)
	[RSP+1618] 0x7FF709DE2DE0     (void* -> SkyrimSE.exe+04F2DE0	xor sil, sil)
	[RSP+1620] 0x1                (size_t) [1]
	[RSP+1628] 0x9EF15FF5         (size_t) [2666618869]
	[RSP+1630] 0x4BF27FFC10       (void*)
	[RSP+1638] 0x7FF7C6627709     (size_t) [140702161991433]
	[RSP+1640] 0x4BF27FFD08       (void*)
	[RSP+1648] 0x4BF27FFD10       (void*)
	[RSP+1650] 0x4BF27FFBE0       (void*)
	[RSP+1658] 0xBCFEDA38         (size_t) [3170818616]
	[RSP+1660] 0x1A22F3CE640      (ScrapHeap*)
	[RSP+1668] 0x1A3A1BB3D68      (void*)
	[RSP+1670] 0xBA9D5E1800000001 (size_t) [uint: 13447007519570395137 int: -4999736554139156479]
	[RSP+1678] 0x7FF700000000     (size_t) [140698833649664]
	[RSP+1680] 0xBC8AC2983EE8AD7C (size_t) [uint: 13585885185062776188 int: -4860858888646775428]
	[RSP+1688] 0x469FF5CF3F63FF24 (size_t) [5089056374422503204]
	[RSP+1690] 0x1AD3557454       (size_t) [115214742612]
	[RSP+1698] 0x4E20             (size_t) [20000]
	[RSP+16A0] 0x0                (size_t) [0]
	[RSP+16A8] 0x0                (size_t) [0]
	[RSP+16B0] 0x0                (size_t) [0]
	[RSP+16B8] 0x7FF70AF0A2B8     (void* -> SkyrimSE.exe+161A2B8	mov eax, 0xF70AD65F)
	[RSP+16C0] 0x4BF27FFBE0       (void*)
	[RSP+16C8] 0x7FF70A5A47EC     (void* -> SkyrimSE.exe+0CB47EC	)
	[RSP+16D0] 0x1A236EF1880      (BSGeometryListCullingProcess*)
	[RSP+16D8] 0xFFFFFFFFFFFFFFFE (size_t) [uint: 18446744073709551614 int: -2]
	[RSP+16E0] 0x0                (size_t) [0]
	[RSP+16E8] 0x0                (size_t) [0]
	[RSP+16F0] 0x0                (size_t) [0]
	[RSP+16F8] 0x7FF70A68C6E1     (void* -> SkyrimSE.exe+0D9C6E1	test rdi, rdi)
	[RSP+1700] 0x1A277345DC0      (BSGeometryListCullingProcess*)
	[RSP+1708] 0x0                (size_t) [0]
	[RSP+1710] 0x1A236EF1880      (BSGeometryListCullingProcess*)
	[RSP+1718] 0x1A39B9ACB80      (BSMultiBoundNode*)
		RTTIName: "BSMultiBoundNode"
		Flags: kSelectiveUpdate | kSelectiveUpdateTransforms | kSelectiveUpdateController
		Checking Parent: 1
			RTTIName: "NiNode"
			Flags: kSelectiveUpdate | kSelectiveUpdateTransforms | kSelectiveUpdateController
			Checking Parent: 2
				RTTIName: "BSMultiBoundNode"
				Flags: kSelectiveUpdate | kSelectiveUpdateTransforms | kSelectiveUpdateController
				Checking Parent: 2
					Name: "ObjectLODRoot"
					RTTIName: "NiNode"
					Flags: kSelectiveUpdate | kSelectiveUpdateTransforms | kSelectiveUpdateController
					Checking Parent: 3
						Name: "shadow scene node"
						RTTIName: "ShadowSceneNode"
						Flags: kSelectiveUpdate | kSelectiveUpdateTransforms | kSelectiveUpdateController
						Checking Parent: 1
							Name: "WorldRoot Node"
							RTTIName: "SceneGraph"
							Flags: kSelectiveUpdate | kSelectiveUpdateTransforms | kSelectiveUpdateController
	[RSP+1720] 0x0                (size_t) [0]
	[RSP+1728] 0x0                (size_t) [0]
	[RSP+1730] 0x0                (size_t) [0]
	[RSP+1738] 0x7FF70C982644     (void* -> SkyrimSE.exe+3092644	add [rax], al)
	[RSP+1740] 0x1                (size_t) [1]
	[RSP+1748] 0x7FF70C982640     (void* -> SkyrimSE.exe+3092640	add [rax], al)
	[RSP+1750] 0x7FF70C982648     (void* -> SkyrimSE.exe+3092648	add [rax], al)
	[RSP+1758] 0x7FF70C8B23D0     (BGSStoryTeller*)
	[RSP+1760] 0x0                (size_t) [0]
	[RSP+1768] 0x1A2383F38E0      (void*)
	[RSP+1770] 0x0                (size_t) [0]
	[RSP+1778] 0x7FF709DE2A45     (void* -> SkyrimSE.exe+04F2A45	mov rdx, rbx)
	[RSP+1780] 0x0                (size_t) [0]
	[RSP+1788] 0x1A22F3CE600      (void*)
	[RSP+1790] 0xFFFFFF00         (size_t) [4294967040]
	[RSP+1798] 0x7FF700000002     (size_t) [140698833649666]
	[RSP+17A0] 0x1A203D4AB00      (void*)
	[RSP+17A8] 0x7FF709F68A56     (void* -> SkyrimSE.exe+0678A56	nop)
	[RSP+17B0] 0x1A2383F38E0      (void*)
	[RSP+17B8] 0x7FF70ACF62CE     (void* -> SkyrimSE.exe+14062CE	mov rcx, rbx)
	[RSP+17C0] 0x7FF70C982644     (void* -> SkyrimSE.exe+3092644	add [rax], al)
	[RSP+17C8] 0xFFFFFFFF         (size_t) [4294967295]
	[RSP+17D0] 0xFFFFFFFFFFFFFFFE (size_t) [uint: 18446744073709551614 int: -2]
	[RSP+17D8] 0x1A203D4BBA0      (void*)
	[RSP+17E0] 0x7FF70C9850E0     (void* -> SkyrimSE.exe+30950E0	add [rbx+0x1A203D4], ch)
	[RSP+17E8] 0x7FF70A55C628     (void* -> SkyrimSE.exe+0C6C628	mov ecx, [rbx+0x0C])
	[RSP+17F0] 0x7FF700000002     (size_t) [140698833649666]
	[RSP+17F8] 0x7FF70C9850E0     (void* -> SkyrimSE.exe+30950E0	add [rbx+0x1A203D4], ch)
	[RSP+1800] 0x0                (size_t) [0]
	[RSP+1808] 0x7FFDCDA670CD     (void* -> KERNELBASE.dll+00670CD	nop [rax+rax*1], eax)
	[RSP+1810] 0x3                (size_t) [3]
	[RSP+1818] 0x7FF70C985070     (BSJobs::JobThread*)
	[RSP+1820] 0x7FF70C985090     (void* -> SkyrimSE.exe+3095090	add [rax], al)
	[RSP+1828] 0x1A203D4AB00      (void*)
	[RSP+1830] 0x7FF70C998300     (void* -> SkyrimSE.exe+30A8300	ret far 0x13)
	[RSP+1838] 0x7FF70A55CBF1     (void* -> SkyrimSE.exe+0C6CBF1	mov r15d, eax)
	[RSP+1840] 0x1                (size_t) [1]
	[RSP+1848] 0x1                (size_t) [1]
	[RSP+1850] 0x0                (size_t) [0]
	[RSP+1858] 0x7FFD60E25D19     (void* -> EngineFixes.dll+0015D19	cmp dword ptr [0x00007FFD60EE5DE8], 0xFFFFFFFF)
	[RSP+1860] 0x1A203D4AB00      (void*)
	[RSP+1868] 0x1                (size_t) [1]
	[RSP+1870] 0x59EB356F6BF3     (size_t) [98866748681203]
	[RSP+1878] 0x7FF70B846F80     (void* -> SkyrimSE.exe+1F56F80	add [rax], al)
	[RSP+1880] 0x1A203D4A860      (void*)
	[RSP+1888] 0x100000006        (size_t) [4294967302]
	[RSP+1890] 0x7FF700000000     (size_t) [140698833649664]
	[RSP+1898] 0x1A203D4A860      (void*)
	[RSP+18A0] 0x48               (size_t) [72]
	[RSP+18A8] 0x7FF700000001     (size_t) [140698833649665]
	[RSP+18B0] 0x0                (size_t) [0]
	[RSP+18B8] 0x0                (size_t) [0]
	[RSP+18C0] 0x0                (size_t) [0]
	[RSP+18C8] 0x0                (size_t) [0]
	[RSP+18D0] 0x0                (size_t) [0]
	[RSP+18D8] 0x0                (size_t) [0]
	[RSP+18E0] 0x0                (size_t) [0]
	[RSP+18E8] 0x0                (size_t) [0]
	[RSP+18F0] 0x0                (size_t) [0]
	[RSP+18F8] 0x0                (size_t) [0]
	[RSP+1900] 0x7FF70C985070     (BSJobs::JobThread*)
	[RSP+1908] 0x7FF70A55AF7A     (void* -> SkyrimSE.exe+0C6AF7A	movzx eax, byte ptr [rbx+0xA74])
	[RSP+1910] 0x7FF70C985001     (void* -> SkyrimSE.exe+3095001	add [rax], al)
	[RSP+1918] 0x0                (size_t) [0]
	[RSP+1920] 0x1                (size_t) [1]
	[RSP+1928] 0x3                (size_t) [3]
	[RSP+1930] 0x7FF70C985070     (BSJobs::JobThread*)
	[RSP+1938] 0x7FF70A535E4D     (void* -> SkyrimSE.exe+0C45E4D	mov rcx, [0x00007FF70C8F6898])
	[RSP+1940] 0x7FF70C8F68F0     (void* -> SkyrimSE.exe+30068F0	add [rax], al)
	[RSP+1948] 0x7FF70C985070     (BSJobs::JobThread*)
	[RSP+1950] 0x0                (size_t) [0]
	[RSP+1958] 0x0                (size_t) [0]
	[RSP+1960] 0x7FF70C985070     (BSJobs::JobThread*)
	[RSP+1968] 0x0                (size_t) [0]
	[RSP+1970] 0x0                (size_t) [0]
	[RSP+1978] 0x7FFDCE6726AD     (void* -> KERNEL32.DLL+00126AD	mov ecx, eax)
	[RSP+1980] 0x0                (size_t) [0]
	[RSP+1988] 0x0                (size_t) [0]
	[RSP+1990] 0x0                (size_t) [0]
	[RSP+1998] 0x0                (size_t) [0]
	[RSP+19A0] 0x0                (size_t) [0]
	[RSP+19A8] 0x7FFDD016AA68     (void* -> ntdll.dll+005AA68	jmp 0x00007FFDD016AA89)
	[RSP+19B0] 0x0                (size_t) [0]
	[RSP+19B8] 0x0                (size_t) [0]
	[RSP+19C0] 0x0                (size_t) [0]
	[RSP+19C8] 0x0                (size_t) [0]
	[RSP+19D0] 0x0                (size_t) [0]
	[RSP+19D8] 0x0                (size_t) [0]
	[RSP+19E0] 0xAC105D0600000000 (size_t) [uint: 12398512054502162432 int: -6048232019207389184]
	[RSP+19E8] 0x0                (size_t) [0]
	[RSP+19F0] 0x4F0FFFFFB30      (size_t) [5433133628208]
	[RSP+19F8] 0x7FFDCDB5BD30     (void* -> KERNELBASE.dll+015BD30	mov [rsp+0x10], rbx)
	[RSP+1A00] 0x4BF27FD6C0       (void*)
	[RSP+1A08] 0xD80001FFF5869780 (size_t) [uint: 15564442511039960960 int: -2882301562669590656]
	[RSP+1A10] 0x7FFD61A5E036     (size_t) [140726241714230]
	[RSP+1A18] 0x4BF27FD6C0       (void*)
	[RSP+1A20] 0x0                (size_t) [0]
	[RSP+1A28] 0x0                (size_t) [0]
	[RSP+1A30] 0x0                (size_t) [0]
	[RSP+1A38] 0x0                (size_t) [0]
	[RSP+1A40] 0x0                (size_t) [0]
	[RSP+1A48] 0x0                (size_t) [0]
	[RSP+1A50] 0x0                (size_t) [0]
	[RSP+1A58] 0x0                (size_t) [0]
	[RSP+1A60] 0x0                (size_t) [0]
	[RSP+1A68] 0x0                (size_t) [0]
	[RSP+1A70] 0x0                (size_t) [0]
	[RSP+1A78] 0x0                (size_t) [0]

MODULES:
	XINPUT1_3.dll                     0x000000400000
	steam_api64.dll                   0x000051380000
	X3DAudio1_7.dll                   0x0000513C0000
	wintrust.dll                      0x01A2390E0000
	SkyrimSE.exe                      0x7FF7098F0000
	nvcuda64.dll                      0x7FFD47350000
	NvCamera64.dll                    0x7FFD47D10000
	d3dcompiler_47_64.dll             0x7FFD48FB0000
	ImmersiveEquipmentDisplays.dll    0x7FFD49750000
	steamclient64.dll                 0x7FFD49CE0000
	JContainers64.dll                 0x7FFD51840000
	CrashLogger.dll                   0x7FFD58520000
	gameoverlayrenderer64.dll         0x7FFD5A730000
	SoundRecordDistributor.dll        0x7FFD5BDE0000
	XAudio2_7.dll                     0x7FFD5BF10000
	QuickLootEE.dll                   0x7FFD5D4A0000
	po3_Tweaks.dll                    0x7FFD5D740000
	SimpleDualSheath.dll              0x7FFD5EBF0000
	po3_SpellPerkItemDistributor.dll  0x7FFD5EC90000
	BetterThirdPersonSelection.dll    0x7FFD5EE00000
	po3_LockVariations.dll            0x7FFD60B60000
	MCMHelper.dll                     0x7FFD60D30000
	EngineFixes.dll                   0x7FFD60E10000
	ResampleDmo.DLL                   0x7FFD63DC0000
	DSOUND.DLL                        0x7FFD64FB0000
	BugFixesSSE.dll                   0x7FFD7DFC0000
	vstdlib_s64.dll                   0x7FFD7E1F0000
	tier0_s64.dll                     0x7FFD7E2B0000
	skse64_1_6_640.dll                0x7FFD7E450000
	bink2w64.dll                      0x7FFD7E580000
	nvspcap64.dll                     0x7FFD7FB70000
	tbbmalloc.dll                     0x7FFD88350000
	tbb.dll                           0x7FFD93F40000
	ncryptsslp.dll                    0x7FFD98700000
	AchievementsModsEnabler.dll       0x7FFD98730000
	msdmo.dll                         0x7FFD98DC0000
	DINPUT8.dll                       0x7FFD9F470000
	MessageBus.dll                    0x7FFDB1CA0000
	nvwgf2umx.dll                     0x7FFDB2B90000
	MpOav.dll                         0x7FFDB8C80000
	webio.dll                         0x7FFDB8D40000
	amsi.dll                          0x7FFDB9300000
	textinputframework.dll            0x7FFDB99B0000
	winmmbase.dll                     0x7FFDB9D30000
	wbemsvc.dll                       0x7FFDBB530000
	rasadhlp.dll                      0x7FFDBB630000
	AUDIOSES.DLL                      0x7FFDBB860000
	fastprox.dll                      0x7FFDBBA90000
	WINMM.dll                         0x7FFDBD2C0000
	Secur32.dll                       0x7FFDBD350000
	MessageBus.dll                    0x7FFDBF490000
	MSVCP140.dll                      0x7FFDC0080000
	XINPUT9_1_0.dll                   0x7FFDC06E0000
	Windows.UI.dll                    0x7FFDC09A0000
	VCRUNTIME140_1.dll                0x7FFDC0B20000
	VCRUNTIME140.dll                  0x7FFDC0B90000
	OneCoreCommonProxyStub.dll        0x7FFDC1060000
	inputhost.dll                     0x7FFDC1A40000
	nvapi64.dll                       0x7FFDC31E0000
	nvldumdx.dll                      0x7FFDC3980000
	OneCoreUAPCommonProxyStub.dll     0x7FFDC4170000
	wbemcomn.dll                      0x7FFDC4FC0000
	wbemprox.dll                      0x7FFDC5AA0000
	MMDevApi.dll                      0x7FFDC5B00000
	drvstore.dll                      0x7FFDC5FA0000
	fwpuclnt.dll                      0x7FFDC6820000
	cryptnet.dll                      0x7FFDC6A00000
	VERSION.dll                       0x7FFDC6A40000
	CoreUIComponents.dll              0x7FFDC6D30000
	dhcpcsvc.DLL                      0x7FFDC7390000
	avrt.dll                          0x7FFDC73D0000
	dhcpcsvc6.DLL                     0x7FFDC7470000
	WINHTTP.dll                       0x7FFDC7490000
	directxdatabasehelper.dll         0x7FFDC75D0000
	MSVCP140_ATOMIC_WAIT.dll          0x7FFDC82B0000
	D3DCOMPILER_47.dll                0x7FFDC8790000
	WindowsCodecs.dll                 0x7FFDC8C30000
	d3d11.dll                         0x7FFDC9620000
	dcomp.dll                         0x7FFDC9880000
	AchievementsModsEnablerLoader.dll 0x7FFDC9B10000
	d3dx9_42.dll                      0x7FFDC9B80000
	CoreMessaging.dll                 0x7FFDCA040000
	uxtheme.dll                       0x7FFDCA590000
	dxgi.dll                          0x7FFDCA6C0000
	dwmapi.dll                        0x7FFDCA7D0000
	WINNSI.DLL                        0x7FFDCA800000
	dxcore.dll                        0x7FFDCA840000
	resourcepolicyclient.dll          0x7FFDCAB80000
	dbghelp.dll                       0x7FFDCAD70000
	wintypes.dll                      0x7FFDCB390000
	windows.storage.dll               0x7FFDCB4D0000
	HID.DLL                           0x7FFDCBDC0000
	IPHLPAPI.DLL                      0x7FFDCC0D0000
	DNSAPI.dll                        0x7FFDCC150000
	UMPDC.dll                         0x7FFDCC3C0000
	powrprof.dll                      0x7FFDCC3E0000
	schannel.DLL                      0x7FFDCC480000
	rsaenh.dll                        0x7FFDCC590000
	kernel.appcore.dll                0x7FFDCC5D0000
	ntmarta.dll                       0x7FFDCC640000
	SSPICLI.DLL                       0x7FFDCC880000
	MSWSOCK.dll                       0x7FFDCCAA0000
	USERENV.dll                       0x7FFDCCB90000
	CRYPTSP.dll                       0x7FFDCCCF0000
	CRYPTBASE.DLL                     0x7FFDCCD10000
	wldp.dll                          0x7FFDCCDA0000
	NTASN1.dll                        0x7FFDCCE20000
	ncrypt.dll                        0x7FFDCCE60000
	bcrypt.dll                        0x7FFDCCE90000
	msasn1.dll                        0x7FFDCD190000
	cfgmgr32.dll                      0x7FFDCD1B0000
	devobj.dll                        0x7FFDCD200000
	DPAPI.DLL                         0x7FFDCD250000
	profapi.dll                       0x7FFDCD420000
	CRYPT32.dll                       0x7FFDCD4F0000
	win32u.dll                        0x7FFDCD660000
	gdi32full.dll                     0x7FFDCD700000
	bcryptPrimitives.dll              0x7FFDCD820000
	msvcp_win.dll                     0x7FFDCD8A0000
	KERNELBASE.dll                    0x7FFDCDA00000
	ucrtbase.dll                      0x7FFDCDDB0000
	SETUPAPI.dll                      0x7FFDCDFD0000
	USER32.dll                        0x7FFDCE450000
	KERNEL32.DLL                      0x7FFDCE660000
	SHLWAPI.dll                       0x7FFDCE730000
	WS2_32.dll                        0x7FFDCE790000
	OLEAUT32.dll                      0x7FFDCE810000
	ole32.dll                         0x7FFDCE960000
	RPCRT4.dll                        0x7FFDCEB00000
	combase.dll                       0x7FFDCEC20000
	msvcrt.dll                        0x7FFDCEFB0000
	PSAPI.DLL                         0x7FFDCF060000
	SHELL32.dll                       0x7FFDCF080000
	imagehlp.dll                      0x7FFDCF8A0000
	sechost.dll                       0x7FFDCF910000
	NSI.dll                           0x7FFDCF9C0000
	ADVAPI32.dll                      0x7FFDCF9F0000
	GDI32.dll                         0x7FFDCFAA0000
	MSCTF.dll                         0x7FFDCFAD0000
	IMM32.DLL                         0x7FFDCFC00000
	clbcatq.dll                       0x7FFDCFCC0000
	SHCORE.dll                        0x7FFDCFFD0000
	ntdll.dll                         0x7FFDD0110000

SKSE PLUGINS:
	AchievementsModsEnablerLoader.dll v1.2
	BetterThirdPersonSelection.dll v1
	BugFixesSSE.dll
	CrashLogger.dll v1.10
	EngineFixes.dll v6.1.1
	ImmersiveEquipmentDisplays.dll v1.7.3
	JContainers64.dll v4.2.3
	MCMHelper.dll v1.4
	po3_LockVariations.dll v3.1.0.1
	po3_SpellPerkItemDistributor.dll v6.6.1.1
	po3_Tweaks.dll v1.8.0.1
	QuickLootEE.dll v1.1
	SimpleDualSheath.dll v1.5.6
	SoundRecordDistributor.dll v1.2

PLUGINS:
	Light: 107	Regular: 51	Total: 158
	[ 0]     Skyrim.esm
	[ 1]     Update.esm
	[ 2]     Dawnguard.esm
	[ 3]     HearthFires.esm
	[ 4]     Dragonborn.esm
	[ 5]     ccBGSSSE001-Fish.esm
	[ 6]     ccBGSSSE025-AdvDSGS.esm
	[ 7]     Unofficial Skyrim Special Edition Patch.esp
	[ 8]     RSkyrimChildren.esm
	[ 9]     MajesticMountains_Landscape.esm
	[ A]     JK's College of Winterhold.esp
	[ B]     3DNPC.esp
	[ C]     Lux Via.esp
	[ D]     Better Dynamic Snow SE - DisableRefs.esm
	[ E]     SkyUI_SE.esp
	[ F]     GQJ_DG_vampireamuletfix.esp
	[10]     Audio Overhaul Skyrim.esp
	[11]     Immersive Sounds - Compendium.esp
	[12]     Prometheus_No_snow_Under_the_roof.esp
	[13]     SMIM-SE-Merged-All.esp
	[14]     Better Dynamic Snow SE.esp
	[15]     LokiHorses.esp
	[16]     SkyHUD.esp
	[17]     Book Covers Skyrim.esp
	[18]     Embers XD.esp
	[19]     JK's Blue Palace.esp
	[1A]     Wintersun - Faiths of Skyrim.esp
	[1B]     Footprints.esp
	[1C]     DeadlySpellImpacts.esp
	[1D]     DeadlySpellImpacts - Two Fire.esp
	[1E]     SpellRituals.esp
	[1F]     Apocalypse - Magic of Skyrim.esp
	[20]     KS Hairdo's.esp
	[21]     IcePenguinWorldMap.esp
	[22]     Fluffworks.esp
	[23]     dD - Enhanced Blood Main.esp
	[24]     PrvtIRoyalArmory.esp
	[25]     Immersive Weapons.esp
	[26]     AVExpansion.esp
	[27]     Draugr Upgrades and Improvements.esp
	[28]     QuickLight.esp
	[29]     FranklyHDImperialArmorsAndWeapons.esp
	[2A]     DIVERSE SKYRIM.esp
	[2B]     Fixed body collision.esp
	[2C]     dynamic fires.esp
	[2D]     RaceMenu.esp
	[2E]     XPMSE.esp
	[2F]     RaceMenuPlugin.esp
	[30]     RSChildren.esp
	[31]     Vokrii - Minimalistic Perks of Skyrim.esp
	[32]     Lux.esp
	[FE:  0] ccQDRSSE001-SurvivalMode.esl
	[FE:  1] ccBGSSSE037-Curios.esl
	[FE:  2] Lux - Resources.esp
	[FE:  3] Lux - Master plugin.esm
	[FE:  4] JK's Understone Keep.esp
	[FE:  5] Lux Via - plugin.esp
	[FE:  6] JK's High Hrothgar.esp
	[FE:  7] JK's Temple of the Divines.esp
	[FE:  8] JK's Sky Haven Temple.esp
	[FE:  9] JK's Arnleif and Sons Trading Company.esp
	[FE:  A] JK's Mistveil Keep.esp
	[FE:  B] JK's Haelga's Bunkhouse.esp
	[FE:  C] JK's Temple of Mara.esp
	[FE:  D] JK's Palace of the Kings.esp
	[FE:  E] JK's Temple of Dibella.esp
	[FE:  F] JK's The Hag's Cure.esp
	[FE: 10] JK's Sinderion's Field Laboratory.esp
	[FE: 11] JK's Dragonsreach.esp
	[FE: 12] JK's Silver-Blood Inn.esp
	[FE: 13] JK's Elgrims Elixirs.esp
	[FE: 14] JK's Bee and Barb.esp
	[FE: 15] MajesticMountains.esp
	[FE: 16] JK's New Gnisis Cornerclub.esp
	[FE: 17] JK's The Pawned Prawn.esp
	[FE: 18] JK's Riverwood Trader.esp
	[FE: 19] JK's Radiant Raiment.esp
	[FE: 1A] JK's White Phial.esp
	[FE: 1B] JK's Sleeping Giant Inn.esp
	[FE: 1C] JK's Angelines Aromatics.esp
	[FE: 1D] JK's Temple of Talos.esp
	[FE: 1E] JK's Candlehearth Hall.esp
	[FE: 1F] JK's The Ragged Flagon.esp
	[FE: 20] JK's Septimus Signus's Outpost.esp
	[FE: 21] JK's Bits and Pieces.esp
	[FE: 22] JK's Warmaiden's.esp
	[FE: 23] JK's Arcadia's Cauldron.esp
	[FE: 24] JK's Sadris Used Wares.esp
	[FE: 25] JK's Temple of Kynareth.esp
	[FE: 26] JKs The Drunken Huntsman.esp
	[FE: 27] Embers XD - Patch - Lux Via.esp
	[FE: 28] CBBE.esp
	[FE: 29] Embers XD - Patch - JKs Dragonsreach.esp
	[FE: 2A] JS Barenziah SE - Johnskyrim.esp
	[FE: 2B] QuickLootEE.esp
	[FE: 2C] Bandit Lines Expansion.esp
	[FE: 2D] MCMHelper.esp
	[FE: 2E] BetterThirdPersonSelection.esp
	[FE: 2F] Headhunter - Bounties Redone.esp
	[FE: 30] Bijin NPCs.esp
	[FE: 31] Bijin Wives.esp
	[FE: 32] Bijin Warmaidens.esp
	[FE: 33] Serana.esp
	[FE: 34] KSHairdosSMP.esp
	[FE: 35] JK's Belethor's General Goods.esp
	[FE: 36] JKs Angelines Aromatics - USSEP Patch.esp
	[FE: 37] JKs Arcadias Cauldron - USSEP Patch.esp
	[FE: 38] JKs Bits and Pieces - USSEP Patch.esp
	[FE: 39] JKs Blue Palace - Immersion Patch.esp
	[FE: 3A] JKs Drunken Huntsman - USSEP Patch.esp
	[FE: 3B] JKs Palace of the Kings - USSEP Patch.esp
	[FE: 3C] JKs Radiant Raiment - USSEP Patch.esp
	[FE: 3D] JKs Radiant Raiment - Immersion Patch.esp
	[FE: 3E] JKs Ragged Flagon - USSEP Patch.esp
	[FE: 3F] JKs Sinderions Field Laboratory - CC - Fishing patch.esp
	[FE: 40] JKs Temple of Talos - USSEP patch.esp
	[FE: 41] JKs Temple of the Divines - USSEP Patch.esp
	[FE: 42] JKs Understone Keep - USSEP patch.esp
	[FE: 43] Lux - CC Fish patch.esp
	[FE: 44] Lux - JK's Bee and Barb patch.esp
	[FE: 45] Lux - JK's Candlehearth Hall patch.esp
	[FE: 46] Lux - USSEP patch.esp
	[FE: 47] Lux - JK's Angelines Aromatics patch.esp
	[FE: 48] Lux - JK's Arcadia's Cauldron patch.esp
	[FE: 49] Lux - JK's Arnleif and Sons Trading Company patch.esp
	[FE: 4A] Lux - JK's Belethor's General Goods patch.esp
	[FE: 4B] Lux - JK's Bits and Pieces patch.esp
	[FE: 4C] Lux - JK's Blood Inn patch.esp
	[FE: 4D] Lux - JK's Blue Palace patch.esp
	[FE: 4E] Lux - JK's College patch.esp
	[FE: 4F] Lux - JK's Dragonsreach patch.esp
	[FE: 50] Lux - JK's Drunken Huntsman patch.esp
	[FE: 51] Lux - JK's Elgrims Elixirs patch.esp
	[FE: 52] Lux - JK's Haelga's Bunkhouse patch.esp
	[FE: 53] Lux - JK's High Hrothgar patch.esp
	[FE: 54] Lux - JK's Mistveil Keep patch.esp
	[FE: 55] Lux - JK's New Gnisis Cornerclub patch.esp
	[FE: 56] Lux - JK's Palace of Kings patch.esp
	[FE: 57] Lux - JK's Pawned Prawn patch.esp
	[FE: 58] Lux - JK's Radiant Raiment patch.esp
	[FE: 59] Lux - JK's Ragged Flagon patch.esp
	[FE: 5A] Lux - JK's Riverwood Trader patch.esp
	[FE: 5B] Lux - JK's Sadris Used Wares patch.esp
	[FE: 5C] Lux - JK's Septimus Signus Outpost patch.esp
	[FE: 5D] Lux - JK's Sinderion's Lab patch.esp
	[FE: 5E] Lux - JK's Sky Haven patch.esp
	[FE: 5F] Lux - JK's Sleeping Giant inn patch.esp
	[FE: 60] Lux - JK's Temple of Dibella patch.esp
	[FE: 61] Lux - JK's Temple of Divines patch.esp
	[FE: 62] Lux - JK's Temple of Kynareth patch.esp
	[FE: 63] Lux - JK's Temple of Mara patch.esp
	[FE: 64] Lux - JK's Temple of Talos patch.esp
	[FE: 65] Lux - JK's The Hag's Cure patch.esp
	[FE: 66] Lux - JK's Understone Keep patch.esp
	[FE: 67] Lux - JK's Warmaidens patch.esp
	[FE: 68] Lux - JK's White Phial patch.esp
	[FE: 69] Lux - Saints and Seducers patch.esp
	[FE: 6A] Lux - Wintersun patch.esp




[2023-09-13 02:49:02.678] [Global] [info] [32380] [main.cpp:58] Log Level: trace
[2023-09-13 02:49:02.678] [Global] [info] [32380] [main.cpp:197] NOTE: This is not a crashlog. Crashlogs have the name crash-[TIMESTAMP].log
[2023-09-13 02:49:02.678] [Global] [info] [32380] [main.cpp:198] CrashLogger 1.10.0.0 Sep  5 2023 00:40:02 is loading...
[2023-09-13 02:49:02.678] [Global] [info] [32380] [CrashHandler.cpp:565] installed crash handlers
[2023-09-13 02:49:02.678] [Global] [info] [32380] [main.cpp:205] CrashLogger has finished loading.
[2023-09-13 02:50:52.623] [Global] [info] [32724] [PdbHandler.cpp:178] Symcache not found at c:\symcache
[2023-09-13 02:50:52.627] [Global] [info] [32724] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+02EDB5A with path Data/SKSE/Plugins
[2023-09-13 02:50:52.647] [Global] [info] [32724] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+02EDB5A	Unable to locate PDB
[2023-09-13 02:50:52.691] [Global] [info] [32724] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+02EDB5A with path Data/SKSE/Plugins
[2023-09-13 02:50:52.691] [Global] [info] [32724] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+02EDB5A	Unable to locate PDB
[2023-09-13 02:50:52.691] [Global] [info] [32724] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+04611EC with path Data/SKSE/Plugins
[2023-09-13 02:50:52.692] [Global] [info] [32724] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+04611EC	Unable to locate PDB
[2023-09-13 02:50:52.692] [Global] [info] [32724] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+04600A4 with path Data/SKSE/Plugins
[2023-09-13 02:50:52.692] [Global] [info] [32724] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+04600A4	Unable to locate PDB
[2023-09-13 02:50:52.692] [Global] [info] [32724] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+0397F6D with path Data/SKSE/Plugins
[2023-09-13 02:50:52.693] [Global] [info] [32724] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+0397F6D	Unable to locate PDB
[2023-09-13 02:50:52.693] [Global] [info] [32724] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+0394861 with path Data/SKSE/Plugins
[2023-09-13 02:50:52.693] [Global] [info] [32724] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+0394861	Unable to locate PDB
[2023-09-13 02:50:52.693] [Global] [info] [32724] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+0390875 with path Data/SKSE/Plugins
[2023-09-13 02:50:52.694] [Global] [info] [32724] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+0390875	Unable to locate PDB
[2023-09-13 02:50:52.694] [Global] [info] [32724] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+038D29D with path Data/SKSE/Plugins
[2023-09-13 02:50:52.694] [Global] [info] [32724] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+038D29D	Unable to locate PDB
[2023-09-13 02:50:52.694] [Global] [info] [32724] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+04EF95C with path Data/SKSE/Plugins
[2023-09-13 02:50:52.695] [Global] [info] [32724] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+04EF95C	Unable to locate PDB
[2023-09-13 02:50:52.695] [Global] [info] [32724] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+04EEFA3 with path Data/SKSE/Plugins
[2023-09-13 02:50:52.695] [Global] [info] [32724] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+04EEFA3	Unable to locate PDB
[2023-09-13 02:50:52.695] [Global] [info] [32724] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+04EECB6 with path Data/SKSE/Plugins
[2023-09-13 02:50:52.696] [Global] [info] [32724] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+04EECB6	Unable to locate PDB
[2023-09-13 02:50:52.696] [Global] [info] [32724] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+04EECB6 with path Data/SKSE/Plugins
[2023-09-13 02:50:52.696] [Global] [info] [32724] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+04EECB6	Unable to locate PDB
[2023-09-13 02:50:52.696] [Global] [info] [32724] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+04EECB6 with path Data/SKSE/Plugins
[2023-09-13 02:50:52.697] [Global] [info] [32724] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+04EECB6	Unable to locate PDB
[2023-09-13 02:50:52.697] [Global] [info] [32724] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+04ECB11 with path Data/SKSE/Plugins
[2023-09-13 02:50:52.697] [Global] [info] [32724] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+04ECB11	Unable to locate PDB
[2023-09-13 02:50:52.697] [Global] [info] [32724] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+04F2DE0 with path Data/SKSE/Plugins
[2023-09-13 02:50:52.698] [Global] [info] [32724] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+04F2DE0	Unable to locate PDB
[2023-09-13 02:50:52.698] [Global] [info] [32724] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+04F2A45 with path Data/SKSE/Plugins
[2023-09-13 02:50:52.698] [Global] [info] [32724] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+04F2A45	Unable to locate PDB
[2023-09-13 02:50:52.698] [Global] [info] [32724] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+0678A56 with path Data/SKSE/Plugins
[2023-09-13 02:50:52.699] [Global] [info] [32724] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+0678A56	Unable to locate PDB
[2023-09-13 02:50:52.699] [Global] [info] [32724] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+0C6C628 with path Data/SKSE/Plugins
[2023-09-13 02:50:52.699] [Global] [info] [32724] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+0C6C628	Unable to locate PDB
[2023-09-13 02:50:52.699] [Global] [info] [32724] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+0C6CBF1 with path Data/SKSE/Plugins
[2023-09-13 02:50:52.699] [Global] [info] [32724] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+0C6CBF1	Unable to locate PDB
[2023-09-13 02:50:52.700] [Global] [info] [32724] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+0C6AF7A with path Data/SKSE/Plugins
[2023-09-13 02:50:52.700] [Global] [info] [32724] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+0C6AF7A	Unable to locate PDB
[2023-09-13 02:50:52.700] [Global] [info] [32724] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+0C45E4D with path Data/SKSE/Plugins
[2023-09-13 02:50:52.700] [Global] [info] [32724] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+0C45E4D	Unable to locate PDB
[2023-09-13 02:50:52.701] [Global] [info] [32724] [PdbHandler.cpp:189] Attempting to find pdb for C:/WINDOWS/System32/KERNEL32.DLL+00126AD with path Data/SKSE/Plugins
[2023-09-13 02:50:52.701] [Global] [info] [32724] [PdbHandler.cpp:193] Failed to open pdb for dll C:/WINDOWS/System32/KERNEL32.DLL+00126AD	Unable to locate PDB
[2023-09-13 02:50:52.701] [Global] [info] [32724] [PdbHandler.cpp:189] Attempting to find pdb for C:/WINDOWS/SYSTEM32/ntdll.dll+005AA68 with path Data/SKSE/Plugins
[2023-09-13 02:50:52.702] [Global] [info] [32724] [PdbHandler.cpp:193] Failed to open pdb for dll C:/WINDOWS/SYSTEM32/ntdll.dll+005AA68	Unable to locate PDB
[2023-09-13 02:50:52.703] [Global] [info] [32724] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+02EDB20 with path Data/SKSE/Plugins
[2023-09-13 02:50:52.703] [Global] [info] [32724] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+02EDB20	Unable to locate PDB
[2023-09-13 02:50:52.703] [Global] [info] [34560] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+2F9AA20 with path Data/SKSE/Plugins
[2023-09-13 02:50:52.703] [Global] [info] [34560] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+2F9AA20	Unable to locate PDB
[2023-09-13 02:50:52.703] [Global] [info] [34548] [Introspection.cpp:1504] Found unhandled type:	(BGSListForm*)	.?AVBGSListForm@@
[2023-09-13 02:50:52.704] [Global] [info] [5640] [Introspection.cpp:1504] Found unhandled type:	(BGSListForm*)	.?AVBGSListForm@@
[2023-09-13 02:50:52.704] [Global] [info] [34548] [Introspection.cpp:1504] Found unhandled type:	(BGSListForm*)	.?AVBaseFormComponent@@
[2023-09-13 02:50:52.704] [Global] [info] [5640] [Introspection.cpp:1504] Found unhandled type:	(BGSListForm*)	.?AVBaseFormComponent@@
[2023-09-13 02:50:52.736] [Global] [info] [34544] [Introspection.cpp:1504] Found unhandled type:	(TESObjectREFR*)	.?AVBaseFormComponent@@
[2023-09-13 02:50:52.736] [Global] [info] [34544] [Introspection.cpp:1504] Found unhandled type:	(TESObjectREFR*)	.?AVBSHandleRefObject@@
[2023-09-13 02:50:52.736] [Global] [info] [34544] [Introspection.cpp:1504] Found unhandled type:	(TESObjectREFR*)	.?AVNiRefObject@@
[2023-09-13 02:50:52.736] [Global] [info] [34544] [Introspection.cpp:1504] Found unhandled type:	(TESObjectREFR*)	.?AV?$BSTEventSink@UBSAnimationGraphEvent@@@@
[2023-09-13 02:50:52.736] [Global] [info] [34544] [Introspection.cpp:1504] Found unhandled type:	(TESObjectREFR*)	.?AVIAnimationGraphManagerHolder@@
[2023-09-13 02:50:52.736] [Global] [info] [32724] [Introspection.cpp:1504] Found unhandled type:	(BGSListForm*)	.?AVBGSListForm@@
[2023-09-13 02:50:52.736] [Global] [info] [34544] [Introspection.cpp:1504] Found unhandled type:	(TESObjectREFR*)	.?AVBaseFormComponent@@
[2023-09-13 02:50:52.736] [Global] [info] [34560] [Introspection.cpp:1504] Found unhandled type:	(BGSListForm*)	.?AVBGSListForm@@
[2023-09-13 02:50:52.736] [Global] [info] [5640] [Introspection.cpp:1504] Found unhandled type:	(TESObjectREFR*)	.?AVBaseFormComponent@@
[2023-09-13 02:50:52.736] [Global] [info] [5640] [Introspection.cpp:1504] Found unhandled type:	(TESObjectREFR*)	.?AVBSHandleRefObject@@
[2023-09-13 02:50:52.736] [Global] [info] [5640] [Introspection.cpp:1504] Found unhandled type:	(TESObjectREFR*)	.?AVNiRefObject@@
[2023-09-13 02:50:52.736] [Global] [info] [5640] [Introspection.cpp:1504] Found unhandled type:	(TESObjectREFR*)	.?AV?$BSTEventSink@UBSAnimationGraphEvent@@@@
[2023-09-13 02:50:52.736] [Global] [info] [5640] [Introspection.cpp:1504] Found unhandled type:	(TESObjectREFR*)	.?AVIAnimationGraphManagerHolder@@
[2023-09-13 02:50:52.736] [Global] [info] [34544] [Introspection.cpp:1504] Found unhandled type:	(TESObjectREFR*)	.?AVBSHandleRefObject@@
[2023-09-13 02:50:52.736] [Global] [info] [34544] [Introspection.cpp:1504] Found unhandled type:	(TESObjectREFR*)	.?AVNiRefObject@@
[2023-09-13 02:50:52.736] [Global] [info] [34544] [Introspection.cpp:1504] Found unhandled type:	(TESObjectREFR*)	.?AV?$BSTEventSink@UBSAnimationGraphEvent@@@@
[2023-09-13 02:50:52.736] [Global] [info] [34544] [Introspection.cpp:1504] Found unhandled type:	(TESObjectREFR*)	.?AVIAnimationGraphManagerHolder@@
[2023-09-13 02:50:52.736] [Global] [info] [34580] [Introspection.cpp:1504] Found unhandled type:	(BGSRefAlias*)	.?AVBGSRefAlias@@
[2023-09-13 02:50:52.736] [Global] [info] [34580] [Introspection.cpp:1504] Found unhandled type:	(BGSRefAlias*)	.?AVBGSBaseAlias@@
[2023-09-13 02:50:52.736] [Global] [info] [26984] [Introspection.cpp:1504] Found unhandled type:	(BSScript::Internal::CodeTasklet*)	.?AVIFuncCallQuery@Internal@BSScript@@
[2023-09-13 02:50:52.736] [Global] [info] [26984] [Introspection.cpp:1504] Found unhandled type:	(BSScript::Internal::CodeTasklet*)	.?AUBSIntrusiveRefCounted@@
[2023-09-13 02:50:52.736] [Global] [info] [23216] [Introspection.cpp:1504] Found unhandled type:	(TESObjectCELL*)	.?AVBaseFormComponent@@
[2023-09-13 02:50:52.736] [Global] [info] [34768] [Introspection.cpp:1504] Found unhandled type:	(hkbBehaviorGraph*)	.?AVhkbBehaviorGraph@@
[2023-09-13 02:50:52.736] [Global] [info] [34768] [Introspection.cpp:1504] Found unhandled type:	(hkbBehaviorGraph*)	.?AVhkbGenerator@@
[2023-09-13 02:50:52.736] [Global] [info] [34548] [Introspection.cpp:1504] Found unhandled type:	(BGSListForm*)	.?AVBGSListForm@@
[2023-09-13 02:50:52.736] [Global] [info] [34768] [Introspection.cpp:1504] Found unhandled type:	(hkbBehaviorGraph*)	.?AVhkbBindable@@
[2023-09-13 02:50:52.736] [Global] [info] [34768] [Introspection.cpp:1504] Found unhandled type:	(hkbBehaviorGraph*)	.?AVhkReferencedObject@@
[2023-09-13 02:50:52.736] [Global] [info] [32404] [Introspection.cpp:1504] Found unhandled type:	(BSScript::Internal::CodeTasklet*)	.?AVIFuncCallQuery@Internal@BSScript@@
[2023-09-13 02:50:52.736] [Global] [info] [32404] [Introspection.cpp:1504] Found unhandled type:	(BSScript::Internal::CodeTasklet*)	.?AUBSIntrusiveRefCounted@@
[2023-09-13 02:50:52.736] [Global] [info] [34548] [Introspection.cpp:1504] Found unhandled type:	(BGSListForm*)	.?AVBaseFormComponent@@
[2023-09-13 02:50:52.736] [Global] [info] [34768] [Introspection.cpp:1504] Found unhandled type:	(hkbBehaviorGraph*)	.?AVhkBaseObject@@
[2023-09-13 02:50:52.736] [Global] [info] [34580] [Introspection.cpp:1504] Found unhandled type:	(hkbStateMachine*)	.?AVhkbStateMachine@@
[2023-09-13 02:50:52.736] [Global] [info] [26996] [Introspection.cpp:1504] Found unhandled type:	(BSTriShape*)	.?AVBSTriShape@@
[2023-09-13 02:50:52.736] [Global] [info] [26996] [Introspection.cpp:1504] Found unhandled type:	(BSTriShape*)	.?AVBSGeometry@@
[2023-09-13 02:50:52.736] [Global] [info] [30372] [Introspection.cpp:1504] Found unhandled type:	(TESObjectREFR*)	.?AVBaseFormComponent@@
[2023-09-13 02:50:52.736] [Global] [info] [34560] [Introspection.cpp:1504] Found unhandled type:	(BGSListForm*)	.?AVBaseFormComponent@@
[2023-09-13 02:50:52.736] [Global] [info] [32724] [Introspection.cpp:1504] Found unhandled type:	(BGSListForm*)	.?AVBaseFormComponent@@
[2023-09-13 02:50:52.736] [Global] [info] [34560] [Introspection.cpp:1504] Found unhandled type:	(Character*)	.?AVActor@@
[2023-09-13 02:50:52.736] [Global] [info] [24832] [Introspection.cpp:1504] Found unhandled type:	(BSTriShape*)	.?AVBSTriShape@@
[2023-09-13 02:50:52.736] [Global] [info] [24832] [Introspection.cpp:1504] Found unhandled type:	(BSTriShape*)	.?AVBSGeometry@@
[2023-09-13 02:50:52.736] [Global] [info] [33280] [Introspection.cpp:1504] Found unhandled type:	(BSScript::Internal::CodeTasklet*)	.?AVIFuncCallQuery@Internal@BSScript@@
[2023-09-13 02:50:52.736] [Global] [info] [33280] [Introspection.cpp:1504] Found unhandled type:	(BSScript::Internal::CodeTasklet*)	.?AUBSIntrusiveRefCounted@@
[2023-09-13 02:50:52.736] [Global] [info] [34460] [Introspection.cpp:1504] Found unhandled type:	(TESObjectREFR*)	.?AVBaseFormComponent@@
[2023-09-13 02:50:52.736] [Global] [info] [34460] [Introspection.cpp:1504] Found unhandled type:	(TESObjectREFR*)	.?AVBSHandleRefObject@@
[2023-09-13 02:50:52.737] [Global] [info] [34460] [Introspection.cpp:1504] Found unhandled type:	(TESObjectREFR*)	.?AVNiRefObject@@
[2023-09-13 02:50:52.736] [Global] [info] [34768] [Introspection.cpp:1504] Found unhandled type:	(BSGeometryListCullingProcess*)	.?AVBSGeometryListCullingProcess@@
[2023-09-13 02:50:52.737] [Global] [info] [34768] [Introspection.cpp:1504] Found unhandled type:	(BSGeometryListCullingProcess*)	.?AVBSCullingProcess@@
[2023-09-13 02:50:52.737] [Global] [info] [34768] [Introspection.cpp:1504] Found unhandled type:	(BSGeometryListCullingProcess*)	.?AVNiCullingProcess@@
[2023-09-13 02:50:52.736] [Global] [info] [29936] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/tbbmalloc.dll+00157C3 with path Data/SKSE/Plugins
[2023-09-13 02:50:52.737] [Global] [info] [33280] [Introspection.cpp:1504] Found unhandled type:	(hkbBehaviorGraph*)	.?AVhkbBehaviorGraph@@
[2023-09-13 02:50:52.736] [Global] [info] [34548] [Introspection.cpp:1504] Found unhandled type:	(hkbManualSelectorGenerator*)	.?AVhkbManualSelectorGenerator@@
[2023-09-13 02:50:52.737] [Global] [info] [34548] [Introspection.cpp:1504] Found unhandled type:	(hkbManualSelectorGenerator*)	.?AVhkbGenerator@@
[2023-09-13 02:50:52.736] [Global] [info] [23216] [Introspection.cpp:1504] Found unhandled type:	(TESObjectCELL*)	.?AVBaseFormComponent@@
[2023-09-13 02:50:52.737] [Global] [info] [30372] [Introspection.cpp:1504] Found unhandled type:	(TESObjectREFR*)	.?AVBSHandleRefObject@@
[2023-09-13 02:50:52.737] [Global] [info] [30372] [Introspection.cpp:1504] Found unhandled type:	(TESObjectREFR*)	.?AVNiRefObject@@
[2023-09-13 02:50:52.737] [Global] [info] [30372] [Introspection.cpp:1504] Found unhandled type:	(TESObjectREFR*)	.?AV?$BSTEventSink@UBSAnimationGraphEvent@@@@
[2023-09-13 02:50:52.737] [Global] [info] [24832] [Introspection.cpp:1504] Found unhandled type:	(BSTriShape*)	.?AVNiObject@@
[2023-09-13 02:50:52.737] [Global] [info] [24832] [Introspection.cpp:1504] Found unhandled type:	(BSTriShape*)	.?AVNiRefObject@@
[2023-09-13 02:50:52.737] [Global] [info] [33280] [Introspection.cpp:1504] Found unhandled type:	(hkbBehaviorGraph*)	.?AVhkbGenerator@@
[2023-09-13 02:50:52.737] [Global] [info] [33280] [Introspection.cpp:1504] Found unhandled type:	(hkbBehaviorGraph*)	.?AVhkbBindable@@
[2023-09-13 02:50:52.737] [Global] [info] [33280] [Introspection.cpp:1504] Found unhandled type:	(hkbBehaviorGraph*)	.?AVhkReferencedObject@@
[2023-09-13 02:50:52.737] [Global] [info] [33280] [Introspection.cpp:1504] Found unhandled type:	(hkbBehaviorGraph*)	.?AVhkBaseObject@@
[2023-09-13 02:50:52.736] [Global] [info] [34560] [Introspection.cpp:1504] Found unhandled type:	(Character*)	.?AVBaseFormComponent@@
[2023-09-13 02:50:52.737] [Global] [info] [34560] [Introspection.cpp:1504] Found unhandled type:	(Character*)	.?AVBSHandleRefObject@@
[2023-09-13 02:50:52.737] [Global] [info] [34560] [Introspection.cpp:1504] Found unhandled type:	(Character*)	.?AVNiRefObject@@
[2023-09-13 02:50:52.737] [Global] [info] [34460] [Introspection.cpp:1504] Found unhandled type:	(TESObjectREFR*)	.?AV?$BSTEventSink@UBSAnimationGraphEvent@@@@
[2023-09-13 02:50:52.737] [Global] [info] [34460] [Introspection.cpp:1504] Found unhandled type:	(TESObjectREFR*)	.?AVIAnimationGraphManagerHolder@@
[2023-09-13 02:50:52.737] [Global] [info] [33280] [Introspection.cpp:1504] Found unhandled type:	(TESQuest*)	.?AVBGSStoryManagerTreeForm@@
[2023-09-13 02:50:52.737] [Global] [info] [23216] [Introspection.cpp:1504] Found unhandled type:	(hkbManualSelectorGenerator*)	.?AVhkbManualSelectorGenerator@@
[2023-09-13 02:50:52.737] [Global] [info] [33280] [Introspection.cpp:1504] Found unhandled type:	(TESQuest*)	.?AVBaseFormComponent@@
[2023-09-13 02:50:52.737] [Global] [info] [23216] [Introspection.cpp:1504] Found unhandled type:	(hkbManualSelectorGenerator*)	.?AVhkbGenerator@@
[2023-09-13 02:50:52.737] [Global] [info] [23216] [Introspection.cpp:1504] Found unhandled type:	(hkbManualSelectorGenerator*)	.?AVhkbBindable@@
[2023-09-13 02:50:52.737] [Global] [info] [34556] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+0C614E2 with path Data/SKSE/Plugins
[2023-09-13 02:50:52.736] [Global] [info] [34580] [Introspection.cpp:1504] Found unhandled type:	(hkbStateMachine*)	.?AVhkbGenerator@@
[2023-09-13 02:50:52.736] [Global] [info] [26996] [Introspection.cpp:1504] Found unhandled type:	(BSTriShape*)	.?AVNiObject@@
[2023-09-13 02:50:52.737] [Global] [info] [26996] [Introspection.cpp:1504] Found unhandled type:	(BSTriShape*)	.?AVNiRefObject@@
[2023-09-13 02:50:52.737] [Global] [info] [30372] [Introspection.cpp:1504] Found unhandled type:	(TESObjectREFR*)	.?AVIAnimationGraphManagerHolder@@
[2023-09-13 02:50:52.737] [Global] [info] [34580] [Introspection.cpp:1504] Found unhandled type:	(hkbStateMachine*)	.?AVhkbBindable@@
[2023-09-13 02:50:52.737] [Global] [info] [26996] [Introspection.cpp:1504] Found unhandled type:	(TESQuest*)	.?AVBGSStoryManagerTreeForm@@
[2023-09-13 02:50:52.737] [Global] [info] [26996] [Introspection.cpp:1504] Found unhandled type:	(TESQuest*)	.?AVBaseFormComponent@@
[2023-09-13 02:50:52.737] [Global] [info] [34404] [Introspection.cpp:1504] Found unhandled type:	(BGSRefAlias*)	.?AVBGSRefAlias@@
[2023-09-13 02:50:52.737] [Global] [info] [34404] [Introspection.cpp:1504] Found unhandled type:	(BGSRefAlias*)	.?AVBGSBaseAlias@@
[2023-09-13 02:50:52.737] [Global] [info] [33280] [Introspection.cpp:1504] Found unhandled type:	(TESQuest*)	.?AVBaseFormComponent@@
[2023-09-13 02:50:52.737] [Global] [info] [34548] [Introspection.cpp:1504] Found unhandled type:	(hkbManualSelectorGenerator*)	.?AVhkbBindable@@
[2023-09-13 02:50:52.737] [Global] [info] [34548] [Introspection.cpp:1504] Found unhandled type:	(hkbManualSelectorGenerator*)	.?AVhkReferencedObject@@
[2023-09-13 02:50:52.737] [Global] [info] [34548] [Introspection.cpp:1504] Found unhandled type:	(hkbManualSelectorGenerator*)	.?AVhkBaseObject@@
[2023-09-13 02:50:52.737] [Global] [info] [26996] [Introspection.cpp:1504] Found unhandled type:	(TESQuest*)	.?AVBaseFormComponent@@
[2023-09-13 02:50:52.737] [Global] [info] [23216] [Introspection.cpp:1504] Found unhandled type:	(hkbManualSelectorGenerator*)	.?AVhkReferencedObject@@
[2023-09-13 02:50:52.737] [Global] [info] [23216] [Introspection.cpp:1504] Found unhandled type:	(hkbManualSelectorGenerator*)	.?AVhkBaseObject@@
[2023-09-13 02:50:52.737] [Global] [info] [34580] [Introspection.cpp:1504] Found unhandled type:	(hkbStateMachine*)	.?AVhkReferencedObject@@
[2023-09-13 02:50:52.737] [Global] [info] [34580] [Introspection.cpp:1504] Found unhandled type:	(hkbStateMachine*)	.?AVhkBaseObject@@
[2023-09-13 02:50:52.737] [Global] [info] [34556] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+0C614E2	Unable to locate PDB
[2023-09-13 02:50:52.737] [Global] [info] [26996] [Introspection.cpp:1504] Found unhandled type:	(BSTCommonLLMessageQueue<BSScript::Internal::FunctionMessage>*)	.?AV?$BSTCommonLLMessageQueue@UFunctionMessage@Internal@BSScript@@@@
[2023-09-13 02:50:52.737] [Global] [info] [34580] [Introspection.cpp:1504] Found unhandled type:	(BGSStoryManagerEventNode*)	.?AVBGSStoryManagerEventNode@@
[2023-09-13 02:50:52.737] [Global] [info] [34580] [Introspection.cpp:1504] Found unhandled type:	(BGSStoryManagerEventNode*)	.?AVBGSStoryManagerBranchNode@@
[2023-09-13 02:50:52.737] [Global] [info] [34556] [Introspection.cpp:1504] Found unhandled type:	(PlayerCharacter*)	.?AVActor@@
[2023-09-13 02:50:52.737] [Global] [info] [32688] [Introspection.cpp:1504] Found unhandled type:	(BGSStoryManagerQuestNode*)	.?AVBGSStoryManagerQuestNode@@
[2023-09-13 02:50:52.737] [Global] [info] [32688] [Introspection.cpp:1504] Found unhandled type:	(BGSStoryManagerQuestNode*)	.?AVBGSStoryManagerNodeBase@@
[2023-09-13 02:50:52.737] [Global] [info] [32688] [Introspection.cpp:1504] Found unhandled type:	(BGSStoryManagerQuestNode*)	.?AVBGSStoryManagerTreeForm@@
[2023-09-13 02:50:52.737] [Global] [info] [23216] [Introspection.cpp:1504] Found unhandled type:	(TESQuest*)	.?AVBGSStoryManagerTreeForm@@
[2023-09-13 02:50:52.737] [Global] [info] [31288] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+135FB48 with path Data/SKSE/Plugins
[2023-09-13 02:50:52.737] [Global] [info] [29940] [Introspection.cpp:1504] Found unhandled type:	(PlayerCharacter*)	.?AVActor@@
[2023-09-13 02:50:52.737] [Global] [info] [32688] [Introspection.cpp:1504] Found unhandled type:	(BGSStoryManagerQuestNode*)	.?AVBaseFormComponent@@
[2023-09-13 02:50:52.737] [Global] [info] [32688] [Introspection.cpp:1504] Found unhandled type:	(BGSStoryManagerQuestFinder*)	.?AVBGSStoryManagerQuestFinder@@
[2023-09-13 02:50:52.737] [Global] [info] [32688] [Introspection.cpp:1504] Found unhandled type:	(BGSStoryManagerQuestFinder*)	.?AVBGSStoryManagerTreeVisitor@@
[2023-09-13 02:50:52.737] [Global] [info] [23216] [Introspection.cpp:1504] Found unhandled type:	(TESQuest*)	.?AVBaseFormComponent@@
[2023-09-13 02:50:52.737] [Global] [info] [23216] [Introspection.cpp:1504] Found unhandled type:	(TESQuest*)	.?AVBaseFormComponent@@
[2023-09-13 02:50:52.737] [Global] [info] [34556] [Introspection.cpp:1504] Found unhandled type:	(PlayerCharacter*)	.?AVBaseFormComponent@@
[2023-09-13 02:50:52.737] [Global] [info] [34556] [Introspection.cpp:1504] Found unhandled type:	(PlayerCharacter*)	.?AVBSHandleRefObject@@
[2023-09-13 02:50:52.737] [Global] [info] [34556] [Introspection.cpp:1504] Found unhandled type:	(PlayerCharacter*)	.?AVNiRefObject@@
[2023-09-13 02:50:52.737] [Global] [info] [34556] [Introspection.cpp:1504] Found unhandled type:	(PlayerCharacter*)	.?AV?$BSTEventSink@UBSAnimationGraphEvent@@@@
[2023-09-13 02:50:52.737] [Global] [info] [34556] [Introspection.cpp:1504] Found unhandled type:	(PlayerCharacter*)	.?AVIAnimationGraphManagerHolder@@
[2023-09-13 02:50:52.737] [Global] [info] [34556] [Introspection.cpp:1504] Found unhandled type:	(PlayerCharacter*)	.?AVMagicTarget@@
[2023-09-13 02:50:52.737] [Global] [info] [34556] [Introspection.cpp:1504] Found unhandled type:	(PlayerCharacter*)	.?AVActorValueOwner@@
[2023-09-13 02:50:52.737] [Global] [info] [34556] [Introspection.cpp:1504] Found unhandled type:	(PlayerCharacter*)	.?AVActorState@@
[2023-09-13 02:50:52.737] [Global] [info] [34580] [Introspection.cpp:1504] Found unhandled type:	(BGSStoryManagerEventNode*)	.?AVBGSStoryManagerNodeBase@@
[2023-09-13 02:50:52.737] [Global] [info] [34580] [Introspection.cpp:1504] Found unhandled type:	(BGSStoryManagerEventNode*)	.?AVBGSStoryManagerTreeForm@@
[2023-09-13 02:50:52.737] [Global] [info] [26996] [Introspection.cpp:1504] Found unhandled type:	(BSTCommonLLMessageQueue<BSScript::Internal::FunctionMessage>*)	.?AV?$BSTCommonMessageQueue@UFunctionMessage@Internal@BSScript@@@@
[2023-09-13 02:50:52.737] [Global] [info] [29940] [Introspection.cpp:1504] Found unhandled type:	(PlayerCharacter*)	.?AVBaseFormComponent@@
[2023-09-13 02:50:52.737] [Global] [info] [29940] [Introspection.cpp:1504] Found unhandled type:	(PlayerCharacter*)	.?AVBSHandleRefObject@@
[2023-09-13 02:50:52.737] [Global] [info] [29940] [Introspection.cpp:1504] Found unhandled type:	(PlayerCharacter*)	.?AVNiRefObject@@
[2023-09-13 02:50:52.737] [Global] [info] [34580] [Introspection.cpp:1504] Found unhandled type:	(BGSStoryManagerEventNode*)	.?AVBaseFormComponent@@
[2023-09-13 02:50:52.738] [Global] [info] [26996] [Introspection.cpp:1504] Found unhandled type:	(BSTCommonLLMessageQueue<BSScript::Internal::FunctionMessage>*)	.?AV?$BSTMessageQueue@UFunctionMessage@Internal@BSScript@@@@
[2023-09-13 02:50:52.737] [Global] [info] [34556] [Introspection.cpp:1504] Found unhandled type:	(PlayerCharacter*)	.?AUIMovementState@@
[2023-09-13 02:50:52.738] [Global] [info] [34556] [Introspection.cpp:1504] Found unhandled type:	(PlayerCharacter*)	.?AUIMovementInterface@@
[2023-09-13 02:50:52.738] [Global] [info] [34556] [Introspection.cpp:1504] Found unhandled type:	(PlayerCharacter*)	.?AV?$BSTEventSink@VBSTransformDeltaEvent@@@@
[2023-09-13 02:50:52.738] [Global] [info] [34556] [Introspection.cpp:1504] Found unhandled type:	(PlayerCharacter*)	.?AV?$BSTEventSink@VbhkCharacterMoveFinishEvent@@@@
[2023-09-13 02:50:52.738] [Global] [info] [34556] [Introspection.cpp:1504] Found unhandled type:	(PlayerCharacter*)	.?AVIPostAnimationChannelUpdateFunctor@@
[2023-09-13 02:50:52.738] [Global] [info] [34556] [Introspection.cpp:1504] Found unhandled type:	(PlayerCharacter*)	.?AV?$BSTEventSource@UBGSActorCellEvent@@@@
[2023-09-13 02:50:52.738] [Global] [info] [34556] [Introspection.cpp:1504] Found unhandled type:	(PlayerCharacter*)	.?AV?$BSTEventSource@UBGSActorDeathEvent@@@@
[2023-09-13 02:50:52.738] [Global] [info] [34556] [Introspection.cpp:1504] Found unhandled type:	(PlayerCharacter*)	.?AV?$BSTEventSource@UPositionPlayerEvent@@@@
[2023-09-13 02:50:52.738] [Global] [info] [34556] [Introspection.cpp:1504] Found unhandled type:	(PlayerCharacter*)	.?AV?$BSTEventSink@VMenuOpenCloseEvent@@@@
[2023-09-13 02:50:52.738] [Global] [info] [34556] [Introspection.cpp:1504] Found unhandled type:	(PlayerCharacter*)	.?AV?$BSTEventSink@VMenuModeChangeEvent@@@@
[2023-09-13 02:50:52.738] [Global] [info] [34524] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+13A383A with path Data/SKSE/Plugins
[2023-09-13 02:50:52.738] [Global] [info] [31288] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+135FB48	Unable to locate PDB
[2023-09-13 02:50:52.737] [Global] [info] [31884] [Introspection.cpp:1504] Found unhandled type:	(BGSStoryManagerQuestNode*)	.?AVBGSStoryManagerQuestNode@@
[2023-09-13 02:50:52.738] [Global] [info] [31884] [Introspection.cpp:1504] Found unhandled type:	(BGSStoryManagerQuestNode*)	.?AVBGSStoryManagerNodeBase@@
[2023-09-13 02:50:52.738] [Global] [info] [31884] [Introspection.cpp:1504] Found unhandled type:	(BGSStoryManagerQuestNode*)	.?AVBGSStoryManagerTreeForm@@
[2023-09-13 02:50:52.738] [Global] [info] [31884] [Introspection.cpp:1504] Found unhandled type:	(BGSStoryManagerQuestNode*)	.?AVBaseFormComponent@@
[2023-09-13 02:50:52.738] [Global] [info] [34560] [Introspection.cpp:1504] Found unhandled type:	(Character*)	.?AV?$BSTEventSink@UBSAnimationGraphEvent@@@@
[2023-09-13 02:50:52.738] [Global] [info] [34560] [Introspection.cpp:1504] Found unhandled type:	(Character*)	.?AVIAnimationGraphManagerHolder@@
[2023-09-13 02:50:52.738] [Global] [info] [34560] [Introspection.cpp:1504] Found unhandled type:	(Character*)	.?AVMagicTarget@@
[2023-09-13 02:50:52.738] [Global] [info] [34560] [Introspection.cpp:1504] Found unhandled type:	(Character*)	.?AVActorValueOwner@@
[2023-09-13 02:50:52.738] [Global] [info] [34560] [Introspection.cpp:1504] Found unhandled type:	(Character*)	.?AVActorState@@
[2023-09-13 02:50:52.738] [Global] [info] [34560] [Introspection.cpp:1504] Found unhandled type:	(Character*)	.?AUIMovementState@@
[2023-09-13 02:50:52.738] [Global] [info] [34560] [Introspection.cpp:1504] Found unhandled type:	(Character*)	.?AUIMovementInterface@@
[2023-09-13 02:50:52.738] [Global] [info] [34560] [Introspection.cpp:1504] Found unhandled type:	(Character*)	.?AV?$BSTEventSink@VBSTransformDeltaEvent@@@@
[2023-09-13 02:50:52.738] [Global] [info] [34560] [Introspection.cpp:1504] Found unhandled type:	(Character*)	.?AV?$BSTEventSink@VbhkCharacterMoveFinishEvent@@@@
[2023-09-13 02:50:52.738] [Global] [info] [34560] [Introspection.cpp:1504] Found unhandled type:	(Character*)	.?AVIPostAnimationChannelUpdateFunctor@@
[2023-09-13 02:50:52.737] [Global] [info] [33644] [Introspection.cpp:1504] Found unhandled type:	(BSTriShape*)	.?AVBSTriShape@@
[2023-09-13 02:50:52.738] [Global] [info] [33644] [Introspection.cpp:1504] Found unhandled type:	(BSTriShape*)	.?AVBSGeometry@@
[2023-09-13 02:50:52.738] [Global] [info] [34556] [Introspection.cpp:1504] Found unhandled type:	(PlayerCharacter*)	.?AV?$BSTEventSink@VUserEventEnabledEvent@@@@
[2023-09-13 02:50:52.738] [Global] [info] [34556] [Introspection.cpp:1504] Found unhandled type:	(PlayerCharacter*)	.?AV?$BSTEventSink@UTESTrackedStatsEvent@@@@
[2023-09-13 02:50:52.738] [Global] [info] [29940] [Introspection.cpp:1504] Found unhandled type:	(PlayerCharacter*)	.?AV?$BSTEventSink@UBSAnimationGraphEvent@@@@
[2023-09-13 02:50:52.738] [Global] [info] [33644] [Introspection.cpp:1504] Found unhandled type:	(BSTriShape*)	.?AVNiObject@@
[2023-09-13 02:50:52.738] [Global] [info] [29940] [Introspection.cpp:1504] Found unhandled type:	(PlayerCharacter*)	.?AVIAnimationGraphManagerHolder@@
[2023-09-13 02:50:52.738] [Global] [info] [33644] [Introspection.cpp:1504] Found unhandled type:	(BSTriShape*)	.?AVNiRefObject@@
[2023-09-13 02:50:52.738] [Global] [info] [34556] [Introspection.cpp:1504] Found unhandled type:	(BGSStoryManagerBranchNode*)	.?AVBGSStoryManagerBranchNode@@
[2023-09-13 02:50:52.738] [Global] [info] [34556] [Introspection.cpp:1504] Found unhandled type:	(BGSStoryManagerBranchNode*)	.?AVBGSStoryManagerNodeBase@@
[2023-09-13 02:50:52.738] [Global] [info] [34556] [Introspection.cpp:1504] Found unhandled type:	(BGSStoryManagerBranchNode*)	.?AVBGSStoryManagerTreeForm@@
[2023-09-13 02:50:52.738] [Global] [info] [34580] [Introspection.cpp:1504] Found unhandled type:	(BGSStoryManagerQuestFinder*)	.?AVBGSStoryManagerQuestFinder@@
[2023-09-13 02:50:52.738] [Global] [info] [34580] [Introspection.cpp:1504] Found unhandled type:	(BGSStoryManagerQuestFinder*)	.?AVBGSStoryManagerTreeVisitor@@
[2023-09-13 02:50:52.738] [Global] [info] [34580] [Introspection.cpp:1504] Found unhandled type:	(BGSStoryManager*)	.?AVBGSStoryManager@@
[2023-09-13 02:50:52.738] [Global] [info] [34580] [Introspection.cpp:1504] Found unhandled type:	(BGSStoryManager*)	.?AU?$BSTSingletonSDM@VBGSStoryManager@@UBSTSingletonSDMOpStaticBuffer@@@@
[2023-09-13 02:50:52.738] [Global] [info] [26008] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+2F9AA00 with path Data/SKSE/Plugins
[2023-09-13 02:50:52.738] [Global] [info] [34560] [Introspection.cpp:1504] Found unhandled type:	(BSGeometryListCullingProcess*)	.?AVBSGeometryListCullingProcess@@
[2023-09-13 02:50:52.738] [Global] [info] [34560] [Introspection.cpp:1504] Found unhandled type:	(BSGeometryListCullingProcess*)	.?AVBSCullingProcess@@
[2023-09-13 02:50:52.738] [Global] [info] [34560] [Introspection.cpp:1504] Found unhandled type:	(BSGeometryListCullingProcess*)	.?AVNiCullingProcess@@
[2023-09-13 02:50:52.738] [Global] [info] [29940] [Introspection.cpp:1504] Found unhandled type:	(PlayerCharacter*)	.?AVMagicTarget@@
[2023-09-13 02:50:52.738] [Global] [info] [29940] [Introspection.cpp:1504] Found unhandled type:	(PlayerCharacter*)	.?AVActorValueOwner@@
[2023-09-13 02:50:52.738] [Global] [info] [34560] [Introspection.cpp:1504] Found unhandled type:	(BGSStoryManagerEventNode*)	.?AVBGSStoryManagerEventNode@@
[2023-09-13 02:50:52.738] [Global] [info] [34560] [Introspection.cpp:1504] Found unhandled type:	(BGSStoryManagerEventNode*)	.?AVBGSStoryManagerBranchNode@@
[2023-09-13 02:50:52.738] [Global] [info] [34560] [Introspection.cpp:1504] Found unhandled type:	(BGSStoryManagerEventNode*)	.?AVBGSStoryManagerNodeBase@@
[2023-09-13 02:50:52.738] [Global] [info] [34560] [Introspection.cpp:1504] Found unhandled type:	(BGSStoryManagerEventNode*)	.?AVBGSStoryManagerTreeForm@@
[2023-09-13 02:50:52.738] [Global] [info] [29940] [Introspection.cpp:1504] Found unhandled type:	(PlayerCharacter*)	.?AVActorState@@
[2023-09-13 02:50:52.738] [Global] [info] [34556] [Introspection.cpp:1504] Found unhandled type:	(BGSStoryManagerBranchNode*)	.?AVBaseFormComponent@@
[2023-09-13 02:50:52.738] [Global] [info] [34580] [Introspection.cpp:1504] Found unhandled type:	(BGSStoryManager*)	.?AU?$BSTSingletonSDMBase@U?$BSTSDMTraits@VBGSStoryManager@@U?$BSTSingletonSDMOpStaticBuffer@VBGSStoryManager@@@@@@@@
[2023-09-13 02:50:52.738] [Global] [info] [34580] [Introspection.cpp:1504] Found unhandled type:	(BGSStoryManager*)	.?AU?$BSTSDMTraits@VBGSStoryManager@@U?$BSTSingletonSDMOpStaticBuffer@VBGSStoryManager@@@@@@
[2023-09-13 02:50:52.738] [Global] [info] [34580] [Introspection.cpp:1504] Found unhandled type:	(BGSStoryManager*)	.?AU?$BSTSingletonSDMOpStaticBuffer@VBGSStoryManager@@@@
[2023-09-13 02:50:52.738] [Global] [info] [34524] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+13A383A	Unable to locate PDB
[2023-09-13 02:50:52.738] [Global] [info] [34560] [Introspection.cpp:1504] Found unhandled type:	(BGSStoryManagerEventNode*)	.?AVBaseFormComponent@@
[2023-09-13 02:50:52.738] [Global] [info] [29940] [Introspection.cpp:1504] Found unhandled type:	(PlayerCharacter*)	.?AUIMovementState@@
[2023-09-13 02:50:52.738] [Global] [info] [29940] [Introspection.cpp:1504] Found unhandled type:	(PlayerCharacter*)	.?AUIMovementInterface@@
[2023-09-13 02:50:52.738] [Global] [info] [29940] [Introspection.cpp:1504] Found unhandled type:	(PlayerCharacter*)	.?AV?$BSTEventSink@VBSTransformDeltaEvent@@@@
[2023-09-13 02:50:52.738] [Global] [info] [34532] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+04600A4 with path Data/SKSE/Plugins
[2023-09-13 02:50:52.738] [Global] [info] [29940] [Introspection.cpp:1504] Found unhandled type:	(PlayerCharacter*)	.?AV?$BSTEventSink@VbhkCharacterMoveFinishEvent@@@@
[2023-09-13 02:50:52.738] [Global] [info] [29940] [Introspection.cpp:1504] Found unhandled type:	(PlayerCharacter*)	.?AVIPostAnimationChannelUpdateFunctor@@
[2023-09-13 02:50:52.738] [Global] [info] [29940] [Introspection.cpp:1504] Found unhandled type:	(PlayerCharacter*)	.?AV?$BSTEventSource@UBGSActorCellEvent@@@@
[2023-09-13 02:50:52.738] [Global] [info] [29940] [Introspection.cpp:1504] Found unhandled type:	(PlayerCharacter*)	.?AV?$BSTEventSource@UBGSActorDeathEvent@@@@
[2023-09-13 02:50:52.738] [Global] [info] [29940] [Introspection.cpp:1504] Found unhandled type:	(PlayerCharacter*)	.?AV?$BSTEventSource@UPositionPlayerEvent@@@@
[2023-09-13 02:50:52.738] [Global] [info] [29940] [Introspection.cpp:1504] Found unhandled type:	(PlayerCharacter*)	.?AV?$BSTEventSink@VMenuOpenCloseEvent@@@@
[2023-09-13 02:50:52.738] [Global] [info] [29940] [Introspection.cpp:1504] Found unhandled type:	(PlayerCharacter*)	.?AV?$BSTEventSink@VMenuModeChangeEvent@@@@
[2023-09-13 02:50:52.738] [Global] [info] [29940] [Introspection.cpp:1504] Found unhandled type:	(PlayerCharacter*)	.?AV?$BSTEventSink@VUserEventEnabledEvent@@@@
[2023-09-13 02:50:52.738] [Global] [info] [26008] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+2F9AA00	Unable to locate PDB
[2023-09-13 02:50:52.738] [Global] [info] [29940] [Introspection.cpp:1504] Found unhandled type:	(PlayerCharacter*)	.?AV?$BSTEventSink@UTESTrackedStatsEvent@@@@
[2023-09-13 02:50:52.738] [Global] [info] [26008] [Introspection.cpp:1504] Found unhandled type:	(BGSStoryManagerBranchNode*)	.?AVBGSStoryManagerBranchNode@@
[2023-09-13 02:50:52.738] [Global] [info] [29940] [Introspection.cpp:1504] Found unhandled type:	(BGSStoryManagerEventNode*)	.?AVBGSStoryManagerEventNode@@
[2023-09-13 02:50:52.738] [Global] [info] [29940] [Introspection.cpp:1504] Found unhandled type:	(BGSStoryManagerEventNode*)	.?AVBGSStoryManagerBranchNode@@
[2023-09-13 02:50:52.738] [Global] [info] [29940] [Introspection.cpp:1504] Found unhandled type:	(BGSStoryManagerEventNode*)	.?AVBGSStoryManagerNodeBase@@
[2023-09-13 02:50:52.738] [Global] [info] [34556] [Introspection.cpp:1504] Found unhandled type:	(BGSStoryManagerQuestFinder*)	.?AVBGSStoryManagerQuestFinder@@
[2023-09-13 02:50:52.738] [Global] [info] [34556] [Introspection.cpp:1504] Found unhandled type:	(BGSStoryManagerQuestFinder*)	.?AVBGSStoryManagerTreeVisitor@@
[2023-09-13 02:50:52.738] [Global] [info] [26008] [Introspection.cpp:1504] Found unhandled type:	(BGSStoryManagerBranchNode*)	.?AVBGSStoryManagerNodeBase@@
[2023-09-13 02:50:52.738] [Global] [info] [26008] [Introspection.cpp:1504] Found unhandled type:	(BGSStoryManagerBranchNode*)	.?AVBGSStoryManagerTreeForm@@
[2023-09-13 02:50:52.738] [Global] [info] [26008] [Introspection.cpp:1504] Found unhandled type:	(BGSStoryManagerBranchNode*)	.?AVBaseFormComponent@@
[2023-09-13 02:50:52.738] [Global] [info] [29940] [Introspection.cpp:1504] Found unhandled type:	(BGSStoryManagerEventNode*)	.?AVBGSStoryManagerTreeForm@@
[2023-09-13 02:50:52.738] [Global] [info] [26008] [Introspection.cpp:1504] Found unhandled type:	(BGSStoryManager*)	.?AVBGSStoryManager@@
[2023-09-13 02:50:52.738] [Global] [info] [29940] [Introspection.cpp:1504] Found unhandled type:	(BGSStoryManagerEventNode*)	.?AVBaseFormComponent@@
[2023-09-13 02:50:52.738] [Global] [info] [26008] [Introspection.cpp:1504] Found unhandled type:	(BGSStoryManager*)	.?AU?$BSTSingletonSDM@VBGSStoryManager@@UBSTSingletonSDMOpStaticBuffer@@@@
[2023-09-13 02:50:52.738] [Global] [info] [26008] [Introspection.cpp:1504] Found unhandled type:	(BGSStoryManager*)	.?AU?$BSTSingletonSDMBase@U?$BSTSDMTraits@VBGSStoryManager@@U?$BSTSingletonSDMOpStaticBuffer@VBGSStoryManager@@@@@@@@
[2023-09-13 02:50:52.738] [Global] [info] [26008] [Introspection.cpp:1504] Found unhandled type:	(BGSStoryManager*)	.?AU?$BSTSDMTraits@VBGSStoryManager@@U?$BSTSingletonSDMOpStaticBuffer@VBGSStoryManager@@@@@@
[2023-09-13 02:50:52.738] [Global] [info] [26008] [Introspection.cpp:1504] Found unhandled type:	(BGSStoryManager*)	.?AU?$BSTSingletonSDMOpStaticBuffer@VBGSStoryManager@@@@
[2023-09-13 02:50:52.738] [Global] [info] [34532] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+04600A4	Unable to locate PDB
[2023-09-13 02:50:52.738] [Global] [info] [34560] [Introspection.cpp:1504] Found unhandled type:	(BGSStoryManagerQuestFinder*)	.?AVBGSStoryManagerQuestFinder@@
[2023-09-13 02:50:52.738] [Global] [info] [34560] [Introspection.cpp:1504] Found unhandled type:	(BGSStoryManagerQuestFinder*)	.?AVBGSStoryManagerTreeVisitor@@
[2023-09-13 02:50:52.738] [Global] [info] [34456] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+161A598 with path Data/SKSE/Plugins
[2023-09-13 02:50:52.739] [Global] [info] [34456] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+161A598	Unable to locate PDB
[2023-09-13 02:50:52.739] [Global] [info] [34456] [Introspection.cpp:1504] Found unhandled type:	(BGSStoryManagerEventNode*)	.?AVBGSStoryManagerEventNode@@
[2023-09-13 02:50:52.739] [Global] [info] [34456] [Introspection.cpp:1504] Found unhandled type:	(BGSStoryManagerEventNode*)	.?AVBGSStoryManagerBranchNode@@
[2023-09-13 02:50:52.739] [Global] [info] [34456] [Introspection.cpp:1504] Found unhandled type:	(BGSStoryManagerEventNode*)	.?AVBGSStoryManagerNodeBase@@
[2023-09-13 02:50:52.739] [Global] [info] [34456] [Introspection.cpp:1504] Found unhandled type:	(BGSStoryManagerEventNode*)	.?AVBGSStoryManagerTreeForm@@
[2023-09-13 02:50:52.739] [Global] [info] [28840] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+1F5CA40 with path Data/SKSE/Plugins
[2023-09-13 02:50:52.739] [Global] [info] [34456] [Introspection.cpp:1504] Found unhandled type:	(BGSStoryManagerEventNode*)	.?AVBaseFormComponent@@
[2023-09-13 02:50:52.739] [Global] [info] [34456] [Introspection.cpp:1504] Found unhandled type:	(BGSStoryManager*)	.?AVBGSStoryManager@@
[2023-09-13 02:50:52.739] [Global] [info] [34456] [Introspection.cpp:1504] Found unhandled type:	(BGSStoryManager*)	.?AU?$BSTSingletonSDM@VBGSStoryManager@@UBSTSingletonSDMOpStaticBuffer@@@@
[2023-09-13 02:50:52.739] [Global] [info] [34456] [Introspection.cpp:1504] Found unhandled type:	(BGSStoryManager*)	.?AU?$BSTSingletonSDMBase@U?$BSTSDMTraits@VBGSStoryManager@@U?$BSTSingletonSDMOpStaticBuffer@VBGSStoryManager@@@@@@@@
[2023-09-13 02:50:52.739] [Global] [info] [34456] [Introspection.cpp:1504] Found unhandled type:	(BGSStoryManager*)	.?AU?$BSTSDMTraits@VBGSStoryManager@@U?$BSTSingletonSDMOpStaticBuffer@VBGSStoryManager@@@@@@
[2023-09-13 02:50:52.739] [Global] [info] [34456] [Introspection.cpp:1504] Found unhandled type:	(BGSStoryManager*)	.?AU?$BSTSingletonSDMOpStaticBuffer@VBGSStoryManager@@@@
[2023-09-13 02:50:52.739] [Global] [info] [34456] [Introspection.cpp:1504] Found unhandled type:	(BGSStoryManagerEventNode*)	.?AVBGSStoryManagerEventNode@@
[2023-09-13 02:50:52.739] [Global] [info] [34456] [Introspection.cpp:1504] Found unhandled type:	(BGSStoryManagerEventNode*)	.?AVBGSStoryManagerBranchNode@@
[2023-09-13 02:50:52.739] [Global] [info] [34456] [Introspection.cpp:1504] Found unhandled type:	(BGSStoryManagerEventNode*)	.?AVBGSStoryManagerNodeBase@@
[2023-09-13 02:50:52.739] [Global] [info] [34456] [Introspection.cpp:1504] Found unhandled type:	(BGSStoryManagerEventNode*)	.?AVBGSStoryManagerTreeForm@@
[2023-09-13 02:50:52.739] [Global] [info] [34456] [Introspection.cpp:1504] Found unhandled type:	(BGSStoryManagerEventNode*)	.?AVBaseFormComponent@@
[2023-09-13 02:50:52.739] [Global] [info] [34456] [Introspection.cpp:1504] Found unhandled type:	(BGSStoryManagerQuestFinder*)	.?AVBGSStoryManagerQuestFinder@@
[2023-09-13 02:50:52.739] [Global] [info] [34456] [Introspection.cpp:1504] Found unhandled type:	(BGSStoryManagerQuestFinder*)	.?AVBGSStoryManagerTreeVisitor@@
[2023-09-13 02:50:52.739] [Global] [info] [28840] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+1F5CA40	Unable to locate PDB
[2023-09-13 02:50:52.739] [Global] [info] [28840] [Introspection.cpp:1504] Found unhandled type:	(ahkpWorld*)	.?AVahkpWorld@@
[2023-09-13 02:50:52.739] [Global] [info] [28840] [Introspection.cpp:1504] Found unhandled type:	(ahkpWorld*)	.?AVhkpWorld@@
[2023-09-13 02:50:52.739] [Global] [info] [28840] [Introspection.cpp:1504] Found unhandled type:	(ahkpWorld*)	.?AVhkReferencedObject@@
[2023-09-13 02:50:52.739] [Global] [info] [28840] [Introspection.cpp:1504] Found unhandled type:	(ahkpWorld*)	.?AVhkBaseObject@@
[2023-09-13 02:50:52.739] [Global] [info] [5640] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+04611EC with path Data/SKSE/Plugins
[2023-09-13 02:50:52.739] [Global] [info] [28840] [Introspection.cpp:1504] Found unhandled type:	(ahkpWorld*)	.?AVahkpWorld@@
[2023-09-13 02:50:52.739] [Global] [info] [28840] [Introspection.cpp:1504] Found unhandled type:	(ahkpWorld*)	.?AVhkpWorld@@
[2023-09-13 02:50:52.739] [Global] [info] [28840] [Introspection.cpp:1504] Found unhandled type:	(ahkpWorld*)	.?AVhkReferencedObject@@
[2023-09-13 02:50:52.739] [Global] [info] [28840] [Introspection.cpp:1504] Found unhandled type:	(ahkpWorld*)	.?AVhkBaseObject@@
[2023-09-13 02:50:52.739] [Global] [info] [5640] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+04611EC	Unable to locate PDB
[2023-09-13 02:50:52.739] [Global] [info] [5640] [Introspection.cpp:1504] Found unhandled type:	(BGSStoryManager*)	.?AVBGSStoryManager@@
[2023-09-13 02:50:52.739] [Global] [info] [5640] [Introspection.cpp:1504] Found unhandled type:	(BGSStoryManager*)	.?AU?$BSTSingletonSDM@VBGSStoryManager@@UBSTSingletonSDMOpStaticBuffer@@@@
[2023-09-13 02:50:52.739] [Global] [info] [5640] [Introspection.cpp:1504] Found unhandled type:	(BGSStoryManager*)	.?AU?$BSTSingletonSDMBase@U?$BSTSDMTraits@VBGSStoryManager@@U?$BSTSingletonSDMOpStaticBuffer@VBGSStoryManager@@@@@@@@
[2023-09-13 02:50:52.739] [Global] [info] [5640] [Introspection.cpp:1504] Found unhandled type:	(BGSStoryManager*)	.?AU?$BSTSDMTraits@VBGSStoryManager@@U?$BSTSingletonSDMOpStaticBuffer@VBGSStoryManager@@@@@@
[2023-09-13 02:50:52.739] [Global] [info] [5640] [Introspection.cpp:1504] Found unhandled type:	(BGSStoryManager*)	.?AU?$BSTSingletonSDMOpStaticBuffer@VBGSStoryManager@@@@
[2023-09-13 02:50:52.739] [Global] [info] [5640] [Introspection.cpp:1504] Found unhandled type:	(BGSStoryManagerEventNode*)	.?AVBGSStoryManagerEventNode@@
[2023-09-13 02:50:52.739] [Global] [info] [5640] [Introspection.cpp:1504] Found unhandled type:	(BGSStoryManagerEventNode*)	.?AVBGSStoryManagerBranchNode@@
[2023-09-13 02:50:52.739] [Global] [info] [5640] [Introspection.cpp:1504] Found unhandled type:	(BGSStoryManagerEventNode*)	.?AVBGSStoryManagerNodeBase@@
[2023-09-13 02:50:52.739] [Global] [info] [5640] [Introspection.cpp:1504] Found unhandled type:	(BGSStoryManagerEventNode*)	.?AVBGSStoryManagerTreeForm@@
[2023-09-13 02:50:52.739] [Global] [info] [34544] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+2FF1570 with path Data/SKSE/Plugins
[2023-09-13 02:50:52.739] [Global] [info] [5640] [Introspection.cpp:1504] Found unhandled type:	(BGSStoryManagerEventNode*)	.?AVBaseFormComponent@@
[2023-09-13 02:50:52.740] [Global] [info] [34544] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+2FF1570	Unable to locate PDB
[2023-09-13 02:50:52.740] [Global] [info] [34552] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+2F9AA88 with path Data/SKSE/Plugins
[2023-09-13 02:50:52.740] [Global] [info] [34544] [Introspection.cpp:1504] Found unhandled type:	(PlayerCharacter*)	.?AVActor@@
[2023-09-13 02:50:52.740] [Global] [info] [34544] [Introspection.cpp:1504] Found unhandled type:	(PlayerCharacter*)	.?AVBaseFormComponent@@
[2023-09-13 02:50:52.740] [Global] [info] [34544] [Introspection.cpp:1504] Found unhandled type:	(PlayerCharacter*)	.?AVBSHandleRefObject@@
[2023-09-13 02:50:52.740] [Global] [info] [34544] [Introspection.cpp:1504] Found unhandled type:	(PlayerCharacter*)	.?AVNiRefObject@@
[2023-09-13 02:50:52.740] [Global] [info] [34544] [Introspection.cpp:1504] Found unhandled type:	(PlayerCharacter*)	.?AV?$BSTEventSink@UBSAnimationGraphEvent@@@@
[2023-09-13 02:50:52.740] [Global] [info] [34544] [Introspection.cpp:1504] Found unhandled type:	(PlayerCharacter*)	.?AVIAnimationGraphManagerHolder@@
[2023-09-13 02:50:52.740] [Global] [info] [34544] [Introspection.cpp:1504] Found unhandled type:	(PlayerCharacter*)	.?AVMagicTarget@@
[2023-09-13 02:50:52.740] [Global] [info] [34544] [Introspection.cpp:1504] Found unhandled type:	(PlayerCharacter*)	.?AVActorValueOwner@@
[2023-09-13 02:50:52.740] [Global] [info] [34544] [Introspection.cpp:1504] Found unhandled type:	(PlayerCharacter*)	.?AVActorState@@
[2023-09-13 02:50:52.740] [Global] [info] [34544] [Introspection.cpp:1504] Found unhandled type:	(PlayerCharacter*)	.?AUIMovementState@@
[2023-09-13 02:50:52.740] [Global] [info] [34544] [Introspection.cpp:1504] Found unhandled type:	(PlayerCharacter*)	.?AUIMovementInterface@@
[2023-09-13 02:50:52.740] [Global] [info] [34544] [Introspection.cpp:1504] Found unhandled type:	(PlayerCharacter*)	.?AV?$BSTEventSink@VBSTransformDeltaEvent@@@@
[2023-09-13 02:50:52.740] [Global] [info] [34544] [Introspection.cpp:1504] Found unhandled type:	(PlayerCharacter*)	.?AV?$BSTEventSink@VbhkCharacterMoveFinishEvent@@@@
[2023-09-13 02:50:52.740] [Global] [info] [34544] [Introspection.cpp:1504] Found unhandled type:	(PlayerCharacter*)	.?AVIPostAnimationChannelUpdateFunctor@@
[2023-09-13 02:50:52.740] [Global] [info] [34544] [Introspection.cpp:1504] Found unhandled type:	(PlayerCharacter*)	.?AV?$BSTEventSource@UBGSActorCellEvent@@@@
[2023-09-13 02:50:52.740] [Global] [info] [34544] [Introspection.cpp:1504] Found unhandled type:	(PlayerCharacter*)	.?AV?$BSTEventSource@UBGSActorDeathEvent@@@@
[2023-09-13 02:50:52.740] [Global] [info] [34544] [Introspection.cpp:1504] Found unhandled type:	(PlayerCharacter*)	.?AV?$BSTEventSource@UPositionPlayerEvent@@@@
[2023-09-13 02:50:52.740] [Global] [info] [34544] [Introspection.cpp:1504] Found unhandled type:	(PlayerCharacter*)	.?AV?$BSTEventSink@VMenuOpenCloseEvent@@@@
[2023-09-13 02:50:52.740] [Global] [info] [34544] [Introspection.cpp:1504] Found unhandled type:	(PlayerCharacter*)	.?AV?$BSTEventSink@VMenuModeChangeEvent@@@@
[2023-09-13 02:50:52.740] [Global] [info] [34544] [Introspection.cpp:1504] Found unhandled type:	(PlayerCharacter*)	.?AV?$BSTEventSink@VUserEventEnabledEvent@@@@
[2023-09-13 02:50:52.740] [Global] [info] [34544] [Introspection.cpp:1504] Found unhandled type:	(PlayerCharacter*)	.?AV?$BSTEventSink@UTESTrackedStatsEvent@@@@
[2023-09-13 02:50:52.740] [Global] [info] [34544] [Introspection.cpp:1504] Found unhandled type:	(PlayerCharacter*)	.?AVActor@@
[2023-09-13 02:50:52.740] [Global] [info] [34544] [Introspection.cpp:1504] Found unhandled type:	(PlayerCharacter*)	.?AVBaseFormComponent@@
[2023-09-13 02:50:52.740] [Global] [info] [34544] [Introspection.cpp:1504] Found unhandled type:	(PlayerCharacter*)	.?AVBSHandleRefObject@@
[2023-09-13 02:50:52.740] [Global] [info] [34544] [Introspection.cpp:1504] Found unhandled type:	(PlayerCharacter*)	.?AVNiRefObject@@
[2023-09-13 02:50:52.740] [Global] [info] [34544] [Introspection.cpp:1504] Found unhandled type:	(PlayerCharacter*)	.?AV?$BSTEventSink@UBSAnimationGraphEvent@@@@
[2023-09-13 02:50:52.740] [Global] [info] [34544] [Introspection.cpp:1504] Found unhandled type:	(PlayerCharacter*)	.?AVIAnimationGraphManagerHolder@@
[2023-09-13 02:50:52.740] [Global] [info] [34544] [Introspection.cpp:1504] Found unhandled type:	(PlayerCharacter*)	.?AVMagicTarget@@
[2023-09-13 02:50:52.740] [Global] [info] [34544] [Introspection.cpp:1504] Found unhandled type:	(PlayerCharacter*)	.?AVActorValueOwner@@
[2023-09-13 02:50:52.740] [Global] [info] [34544] [Introspection.cpp:1504] Found unhandled type:	(PlayerCharacter*)	.?AVActorState@@
[2023-09-13 02:50:52.740] [Global] [info] [34544] [Introspection.cpp:1504] Found unhandled type:	(PlayerCharacter*)	.?AUIMovementState@@
[2023-09-13 02:50:52.740] [Global] [info] [34544] [Introspection.cpp:1504] Found unhandled type:	(PlayerCharacter*)	.?AUIMovementInterface@@
[2023-09-13 02:50:52.740] [Global] [info] [34544] [Introspection.cpp:1504] Found unhandled type:	(PlayerCharacter*)	.?AV?$BSTEventSink@VBSTransformDeltaEvent@@@@
[2023-09-13 02:50:52.740] [Global] [info] [34544] [Introspection.cpp:1504] Found unhandled type:	(PlayerCharacter*)	.?AV?$BSTEventSink@VbhkCharacterMoveFinishEvent@@@@
[2023-09-13 02:50:52.740] [Global] [info] [34544] [Introspection.cpp:1504] Found unhandled type:	(PlayerCharacter*)	.?AVIPostAnimationChannelUpdateFunctor@@
[2023-09-13 02:50:52.740] [Global] [info] [34544] [Introspection.cpp:1504] Found unhandled type:	(PlayerCharacter*)	.?AV?$BSTEventSource@UBGSActorCellEvent@@@@
[2023-09-13 02:50:52.740] [Global] [info] [34544] [Introspection.cpp:1504] Found unhandled type:	(PlayerCharacter*)	.?AV?$BSTEventSource@UBGSActorDeathEvent@@@@
[2023-09-13 02:50:52.740] [Global] [info] [34544] [Introspection.cpp:1504] Found unhandled type:	(PlayerCharacter*)	.?AV?$BSTEventSource@UPositionPlayerEvent@@@@
[2023-09-13 02:50:52.740] [Global] [info] [34544] [Introspection.cpp:1504] Found unhandled type:	(PlayerCharacter*)	.?AV?$BSTEventSink@VMenuOpenCloseEvent@@@@
[2023-09-13 02:50:52.740] [Global] [info] [34544] [Introspection.cpp:1504] Found unhandled type:	(PlayerCharacter*)	.?AV?$BSTEventSink@VMenuModeChangeEvent@@@@
[2023-09-13 02:50:52.740] [Global] [info] [34544] [Introspection.cpp:1504] Found unhandled type:	(PlayerCharacter*)	.?AV?$BSTEventSink@VUserEventEnabledEvent@@@@
[2023-09-13 02:50:52.740] [Global] [info] [34544] [Introspection.cpp:1504] Found unhandled type:	(PlayerCharacter*)	.?AV?$BSTEventSink@UTESTrackedStatsEvent@@@@
[2023-09-13 02:50:52.740] [Global] [info] [34552] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+2F9AA88	Unable to locate PDB
[2023-09-13 02:50:52.740] [Global] [info] [17392] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+2F9AA20 with path Data/SKSE/Plugins
[2023-09-13 02:50:52.740] [Global] [info] [17392] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+2F9AA20	Unable to locate PDB
[2023-09-13 02:50:52.740] [Global] [info] [17392] [Introspection.cpp:1504] Found unhandled type:	(BSTriShape*)	.?AVBSTriShape@@
[2023-09-13 02:50:52.740] [Global] [info] [17392] [Introspection.cpp:1504] Found unhandled type:	(BSTriShape*)	.?AVBSGeometry@@
[2023-09-13 02:50:52.740] [Global] [info] [34280] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+0394861 with path Data/SKSE/Plugins
[2023-09-13 02:50:52.740] [Global] [info] [17392] [Introspection.cpp:1504] Found unhandled type:	(BSTriShape*)	.?AVNiObject@@
[2023-09-13 02:50:52.740] [Global] [info] [17392] [Introspection.cpp:1504] Found unhandled type:	(BSTriShape*)	.?AVNiRefObject@@
[2023-09-13 02:50:52.741] [Global] [info] [34280] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+0394861	Unable to locate PDB
[2023-09-13 02:50:52.741] [Global] [info] [34476] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+2F9AA20 with path Data/SKSE/Plugins
[2023-09-13 02:50:52.741] [Global] [info] [34476] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+2F9AA20	Unable to locate PDB
[2023-09-13 02:50:52.741] [Global] [info] [29412] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+2F9AA20 with path Data/SKSE/Plugins
[2023-09-13 02:50:52.741] [Global] [info] [29412] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+2F9AA20	Unable to locate PDB
[2023-09-13 02:50:52.741] [Global] [info] [30192] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+2F9AA20 with path Data/SKSE/Plugins
[2023-09-13 02:50:52.741] [Global] [info] [29412] [Introspection.cpp:1504] Found unhandled type:	(BSGeometryListCullingProcess*)	.?AVBSGeometryListCullingProcess@@
[2023-09-13 02:50:52.741] [Global] [info] [29412] [Introspection.cpp:1504] Found unhandled type:	(BSGeometryListCullingProcess*)	.?AVBSCullingProcess@@
[2023-09-13 02:50:52.741] [Global] [info] [29412] [Introspection.cpp:1504] Found unhandled type:	(BSGeometryListCullingProcess*)	.?AVNiCullingProcess@@
[2023-09-13 02:50:52.741] [Global] [info] [29412] [Introspection.cpp:1504] Found unhandled type:	(NiNode*)	.?AVNiNode@@
[2023-09-13 02:50:52.741] [Global] [info] [29412] [Introspection.cpp:1504] Found unhandled type:	(NiNode*)	.?AVNiObject@@
[2023-09-13 02:50:52.741] [Global] [info] [29412] [Introspection.cpp:1504] Found unhandled type:	(NiNode*)	.?AVNiRefObject@@
[2023-09-13 02:50:52.741] [Global] [info] [29412] [Introspection.cpp:1504] Found unhandled type:	(BSGeometryListCullingProcess*)	.?AVBSGeometryListCullingProcess@@
[2023-09-13 02:50:52.741] [Global] [info] [29412] [Introspection.cpp:1504] Found unhandled type:	(BSGeometryListCullingProcess*)	.?AVBSCullingProcess@@
[2023-09-13 02:50:52.741] [Global] [info] [29412] [Introspection.cpp:1504] Found unhandled type:	(BSGeometryListCullingProcess*)	.?AVNiCullingProcess@@
[2023-09-13 02:50:52.741] [Global] [info] [30192] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+2F9AA20	Unable to locate PDB
[2023-09-13 02:50:52.741] [Global] [info] [34528] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+2F9AA20 with path Data/SKSE/Plugins
[2023-09-13 02:50:52.742] [Global] [info] [34528] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+2F9AA20	Unable to locate PDB
[2023-09-13 02:50:52.742] [Global] [info] [34528] [Introspection.cpp:1504] Found unhandled type:	(BSMultiBoundNode*)	.?AVBSMultiBoundNode@@
[2023-09-13 02:50:52.742] [Global] [info] [34528] [Introspection.cpp:1504] Found unhandled type:	(BSMultiBoundNode*)	.?AVBSNiNode@@
[2023-09-13 02:50:52.742] [Global] [info] [34528] [Introspection.cpp:1504] Found unhandled type:	(BSMultiBoundNode*)	.?AVNiNode@@
[2023-09-13 02:50:52.742] [Global] [info] [33444] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+1F5CA40 with path Data/SKSE/Plugins
[2023-09-13 02:50:52.742] [Global] [info] [34528] [Introspection.cpp:1504] Found unhandled type:	(BSMultiBoundNode*)	.?AVNiObject@@
[2023-09-13 02:50:52.742] [Global] [info] [34528] [Introspection.cpp:1504] Found unhandled type:	(BSMultiBoundNode*)	.?AVNiRefObject@@
[2023-09-13 02:50:52.742] [Global] [info] [34528] [Introspection.cpp:1504] Found unhandled type:	(BSTriShape*)	.?AVBSTriShape@@
[2023-09-13 02:50:52.742] [Global] [info] [34528] [Introspection.cpp:1504] Found unhandled type:	(BSTriShape*)	.?AVBSGeometry@@
[2023-09-13 02:50:52.742] [Global] [info] [34528] [Introspection.cpp:1504] Found unhandled type:	(BSTriShape*)	.?AVNiObject@@
[2023-09-13 02:50:52.742] [Global] [info] [34528] [Introspection.cpp:1504] Found unhandled type:	(BSTriShape*)	.?AVNiRefObject@@
[2023-09-13 02:50:52.742] [Global] [info] [33444] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+1F5CA40	Unable to locate PDB
[2023-09-13 02:50:52.742] [Global] [info] [29804] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+0397F6D with path Data/SKSE/Plugins
[2023-09-13 02:50:52.742] [Global] [info] [29804] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+0397F6D	Unable to locate PDB
[2023-09-13 02:50:52.742] [Global] [info] [31588] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+0B9F79D with path Data/SKSE/Plugins
[2023-09-13 02:50:52.743] [Global] [info] [31588] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+0B9F79D	Unable to locate PDB
[2023-09-13 02:50:52.743] [Global] [info] [26984] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+13A3A8C with path Data/SKSE/Plugins
[2023-09-13 02:50:52.743] [Global] [info] [31588] [Introspection.cpp:1504] Found unhandled type:	(BSAnimationGraphManager*)	.?AVBSAnimationGraphManager@@
[2023-09-13 02:50:52.743] [Global] [info] [31588] [Introspection.cpp:1504] Found unhandled type:	(BSAnimationGraphManager*)	.?AV?$BSTEventSink@UBSAnimationGraphEvent@@@@
[2023-09-13 02:50:52.743] [Global] [info] [31588] [Introspection.cpp:1504] Found unhandled type:	(BSAnimationGraphManager*)	.?AUBSIntrusiveRefCounted@@
[2023-09-13 02:50:52.743] [Global] [info] [26984] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+13A3A8C	Unable to locate PDB
[2023-09-13 02:50:52.743] [Global] [info] [34344] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+0C6276D with path Data/SKSE/Plugins
[2023-09-13 02:50:52.743] [Global] [info] [34344] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+0C6276D	Unable to locate PDB
[2023-09-13 02:50:52.743] [Global] [info] [34344] [Introspection.cpp:1504] Found unhandled type:	(bhkCharRigidBodyController*)	.?AVbhkCharRigidBodyController@@
[2023-09-13 02:50:52.743] [Global] [info] [34344] [Introspection.cpp:1504] Found unhandled type:	(bhkCharRigidBodyController*)	.?AVbhkCharacterController@@
[2023-09-13 02:50:52.743] [Global] [info] [34344] [Introspection.cpp:1504] Found unhandled type:	(bhkCharRigidBodyController*)	.?AVNiRefObject@@
[2023-09-13 02:50:52.743] [Global] [info] [34344] [Introspection.cpp:1504] Found unhandled type:	(bhkCharRigidBodyController*)	.?AV?$BSTEventSource@VbhkCharacterMoveFinishEvent@@@@
[2023-09-13 02:50:52.743] [Global] [info] [34344] [Introspection.cpp:1504] Found unhandled type:	(bhkCharRigidBodyController*)	.?AVhkpCharacterRigidBodyListener@@
[2023-09-13 02:50:52.743] [Global] [info] [34344] [Introspection.cpp:1504] Found unhandled type:	(bhkCharRigidBodyController*)	.?AVhkReferencedObject@@
[2023-09-13 02:50:52.743] [Global] [info] [34584] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+0C6276D with path Data/SKSE/Plugins
[2023-09-13 02:50:52.743] [Global] [info] [34344] [Introspection.cpp:1504] Found unhandled type:	(bhkCharRigidBodyController*)	.?AVhkBaseObject@@
[2023-09-13 02:50:52.743] [Global] [info] [34344] [Introspection.cpp:1504] Found unhandled type:	(Character*)	.?AVActor@@
[2023-09-13 02:50:52.743] [Global] [info] [34344] [Introspection.cpp:1504] Found unhandled type:	(Character*)	.?AVBaseFormComponent@@
[2023-09-13 02:50:52.743] [Global] [info] [34344] [Introspection.cpp:1504] Found unhandled type:	(Character*)	.?AVBSHandleRefObject@@
[2023-09-13 02:50:52.743] [Global] [info] [34344] [Introspection.cpp:1504] Found unhandled type:	(Character*)	.?AVNiRefObject@@
[2023-09-13 02:50:52.743] [Global] [info] [34344] [Introspection.cpp:1504] Found unhandled type:	(Character*)	.?AV?$BSTEventSink@UBSAnimationGraphEvent@@@@
[2023-09-13 02:50:52.743] [Global] [info] [34344] [Introspection.cpp:1504] Found unhandled type:	(Character*)	.?AVIAnimationGraphManagerHolder@@
[2023-09-13 02:50:52.743] [Global] [info] [34344] [Introspection.cpp:1504] Found unhandled type:	(Character*)	.?AVMagicTarget@@
[2023-09-13 02:50:52.743] [Global] [info] [34344] [Introspection.cpp:1504] Found unhandled type:	(Character*)	.?AVActorValueOwner@@
[2023-09-13 02:50:52.743] [Global] [info] [34344] [Introspection.cpp:1504] Found unhandled type:	(Character*)	.?AVActorState@@
[2023-09-13 02:50:52.743] [Global] [info] [34344] [Introspection.cpp:1504] Found unhandled type:	(Character*)	.?AUIMovementState@@
[2023-09-13 02:50:52.743] [Global] [info] [34344] [Introspection.cpp:1504] Found unhandled type:	(Character*)	.?AUIMovementInterface@@
[2023-09-13 02:50:52.743] [Global] [info] [34344] [Introspection.cpp:1504] Found unhandled type:	(Character*)	.?AV?$BSTEventSink@VBSTransformDeltaEvent@@@@
[2023-09-13 02:50:52.743] [Global] [info] [34344] [Introspection.cpp:1504] Found unhandled type:	(Character*)	.?AV?$BSTEventSink@VbhkCharacterMoveFinishEvent@@@@
[2023-09-13 02:50:52.743] [Global] [info] [34344] [Introspection.cpp:1504] Found unhandled type:	(Character*)	.?AVIPostAnimationChannelUpdateFunctor@@
[2023-09-13 02:50:52.743] [Global] [info] [34344] [Introspection.cpp:1504] Found unhandled type:	(Character*)	.?AVActor@@
[2023-09-13 02:50:52.743] [Global] [info] [34344] [Introspection.cpp:1504] Found unhandled type:	(Character*)	.?AVBaseFormComponent@@
[2023-09-13 02:50:52.743] [Global] [info] [34344] [Introspection.cpp:1504] Found unhandled type:	(Character*)	.?AVBSHandleRefObject@@
[2023-09-13 02:50:52.743] [Global] [info] [34344] [Introspection.cpp:1504] Found unhandled type:	(Character*)	.?AVNiRefObject@@
[2023-09-13 02:50:52.743] [Global] [info] [34344] [Introspection.cpp:1504] Found unhandled type:	(Character*)	.?AV?$BSTEventSink@UBSAnimationGraphEvent@@@@
[2023-09-13 02:50:52.743] [Global] [info] [34344] [Introspection.cpp:1504] Found unhandled type:	(Character*)	.?AVIAnimationGraphManagerHolder@@
[2023-09-13 02:50:52.743] [Global] [info] [34344] [Introspection.cpp:1504] Found unhandled type:	(Character*)	.?AVMagicTarget@@
[2023-09-13 02:50:52.743] [Global] [info] [34344] [Introspection.cpp:1504] Found unhandled type:	(Character*)	.?AVActorValueOwner@@
[2023-09-13 02:50:52.743] [Global] [info] [34344] [Introspection.cpp:1504] Found unhandled type:	(Character*)	.?AVActorState@@
[2023-09-13 02:50:52.743] [Global] [info] [34344] [Introspection.cpp:1504] Found unhandled type:	(Character*)	.?AUIMovementState@@
[2023-09-13 02:50:52.743] [Global] [info] [34344] [Introspection.cpp:1504] Found unhandled type:	(Character*)	.?AUIMovementInterface@@
[2023-09-13 02:50:52.743] [Global] [info] [34344] [Introspection.cpp:1504] Found unhandled type:	(Character*)	.?AV?$BSTEventSink@VBSTransformDeltaEvent@@@@
[2023-09-13 02:50:52.743] [Global] [info] [34344] [Introspection.cpp:1504] Found unhandled type:	(Character*)	.?AV?$BSTEventSink@VbhkCharacterMoveFinishEvent@@@@
[2023-09-13 02:50:52.743] [Global] [info] [34344] [Introspection.cpp:1504] Found unhandled type:	(Character*)	.?AVIPostAnimationChannelUpdateFunctor@@
[2023-09-13 02:50:52.743] [Global] [info] [34584] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+0C6276D	Unable to locate PDB
[2023-09-13 02:50:52.743] [Global] [info] [34584] [Introspection.cpp:1504] Found unhandled type:	(BSAnimationGraphManager*)	.?AVBSAnimationGraphManager@@
[2023-09-13 02:50:52.743] [Global] [info] [34584] [Introspection.cpp:1504] Found unhandled type:	(BSAnimationGraphManager*)	.?AV?$BSTEventSink@UBSAnimationGraphEvent@@@@
[2023-09-13 02:50:52.743] [Global] [info] [34584] [Introspection.cpp:1504] Found unhandled type:	(BSAnimationGraphManager*)	.?AUBSIntrusiveRefCounted@@
[2023-09-13 02:50:52.743] [Global] [info] [27660] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+2FF7860 with path Data/SKSE/Plugins
[2023-09-13 02:50:52.744] [Global] [info] [32404] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/tbbmalloc.dll+0013911 with path Data/SKSE/Plugins
[2023-09-13 02:50:52.744] [Global] [info] [27660] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+2FF7860	Unable to locate PDB
[2023-09-13 02:50:52.744] [Global] [info] [27660] [Introspection.cpp:1504] Found unhandled type:	(hkbFootIkDriver*)	.?AVhkbFootIkDriver@@
[2023-09-13 02:50:52.744] [Global] [info] [27660] [Introspection.cpp:1504] Found unhandled type:	(hkbFootIkDriver*)	.?AVhkReferencedObject@@
[2023-09-13 02:50:52.744] [Global] [info] [27660] [Introspection.cpp:1504] Found unhandled type:	(hkbFootIkDriver*)	.?AVhkBaseObject@@
[2023-09-13 02:50:52.744] [Global] [info] [32488] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+135FCFC with path Data/SKSE/Plugins
[2023-09-13 02:50:52.744] [Global] [info] [32488] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+135FCFC	Unable to locate PDB
[2023-09-13 02:50:52.744] [Global] [info] [32488] [Introspection.cpp:1504] Found unhandled type:	(BSLeafAnimNode*)	.?AVBSLeafAnimNode@@
[2023-09-13 02:50:52.744] [Global] [info] [32488] [Introspection.cpp:1504] Found unhandled type:	(BSLeafAnimNode*)	.?AVBSFadeNode@@
[2023-09-13 02:50:52.744] [Global] [info] [32488] [Introspection.cpp:1504] Found unhandled type:	(BSLeafAnimNode*)	.?AVNiNode@@
[2023-09-13 02:50:52.744] [Global] [info] [28656] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+0CAC998 with path Data/SKSE/Plugins
[2023-09-13 02:50:52.744] [Global] [info] [32488] [Introspection.cpp:1504] Found unhandled type:	(BSLeafAnimNode*)	.?AVNiObject@@
[2023-09-13 02:50:52.744] [Global] [info] [32488] [Introspection.cpp:1504] Found unhandled type:	(BSLeafAnimNode*)	.?AVNiRefObject@@
[2023-09-13 02:50:52.744] [Global] [info] [28656] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+0CAC998	Unable to locate PDB
[2023-09-13 02:50:52.745] [Global] [info] [25836] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+161A598 with path Data/SKSE/Plugins
[2023-09-13 02:50:52.745] [Global] [info] [25836] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+161A598	Unable to locate PDB
[2023-09-13 02:50:52.745] [Global] [info] [34768] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+0D9C421 with path Data/SKSE/Plugins
[2023-09-13 02:50:52.745] [Global] [info] [34768] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+0D9C421	Unable to locate PDB
[2023-09-13 02:50:52.745] [Global] [info] [34460] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+0C6276D with path Data/SKSE/Plugins
[2023-09-13 02:50:52.745] [Global] [info] [34460] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+0C6276D	Unable to locate PDB
[2023-09-13 02:50:52.745] [Global] [info] [34460] [Introspection.cpp:1504] Found unhandled type:	(BSGeometryListCullingProcess*)	.?AVBSGeometryListCullingProcess@@
[2023-09-13 02:50:52.745] [Global] [info] [34460] [Introspection.cpp:1504] Found unhandled type:	(BSGeometryListCullingProcess*)	.?AVBSCullingProcess@@
[2023-09-13 02:50:52.745] [Global] [info] [34460] [Introspection.cpp:1504] Found unhandled type:	(BSGeometryListCullingProcess*)	.?AVNiCullingProcess@@
[2023-09-13 02:50:52.745] [Global] [info] [34460] [Introspection.cpp:1504] Found unhandled type:	(BSFadeNode*)	.?AVBSFadeNode@@
[2023-09-13 02:50:52.745] [Global] [info] [34460] [Introspection.cpp:1504] Found unhandled type:	(BSFadeNode*)	.?AVNiNode@@
[2023-09-13 02:50:52.745] [Global] [info] [34776] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+2F9AA20 with path Data/SKSE/Plugins
[2023-09-13 02:50:52.745] [Global] [info] [34460] [Introspection.cpp:1504] Found unhandled type:	(BSFadeNode*)	.?AVNiObject@@
[2023-09-13 02:50:52.745] [Global] [info] [34460] [Introspection.cpp:1504] Found unhandled type:	(BSFadeNode*)	.?AVNiRefObject@@
[2023-09-13 02:50:52.745] [Global] [info] [34460] [Introspection.cpp:1504] Found unhandled type:	(BSGeometryListCullingProcess*)	.?AVBSGeometryListCullingProcess@@
[2023-09-13 02:50:52.745] [Global] [info] [34460] [Introspection.cpp:1504] Found unhandled type:	(BSGeometryListCullingProcess*)	.?AVBSCullingProcess@@
[2023-09-13 02:50:52.745] [Global] [info] [34460] [Introspection.cpp:1504] Found unhandled type:	(BSGeometryListCullingProcess*)	.?AVNiCullingProcess@@
[2023-09-13 02:50:52.746] [Global] [info] [34776] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+2F9AA20	Unable to locate PDB
[2023-09-13 02:50:52.746] [Global] [info] [34776] [Introspection.cpp:1504] Found unhandled type:	(BSFadeNode*)	.?AVBSFadeNode@@
[2023-09-13 02:50:52.746] [Global] [info] [34776] [Introspection.cpp:1504] Found unhandled type:	(BSFadeNode*)	.?AVNiNode@@
[2023-09-13 02:50:52.746] [Global] [info] [24832] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+0DA440F with path Data/SKSE/Plugins
[2023-09-13 02:50:52.746] [Global] [info] [34776] [Introspection.cpp:1504] Found unhandled type:	(BSFadeNode*)	.?AVNiObject@@
[2023-09-13 02:50:52.746] [Global] [info] [34776] [Introspection.cpp:1504] Found unhandled type:	(BSFadeNode*)	.?AVNiRefObject@@
[2023-09-13 02:50:52.746] [Global] [info] [34776] [Introspection.cpp:1504] Found unhandled type:	(BSGeometryListCullingProcess*)	.?AVBSGeometryListCullingProcess@@
[2023-09-13 02:50:52.746] [Global] [info] [34776] [Introspection.cpp:1504] Found unhandled type:	(BSGeometryListCullingProcess*)	.?AVBSCullingProcess@@
[2023-09-13 02:50:52.746] [Global] [info] [34776] [Introspection.cpp:1504] Found unhandled type:	(BSGeometryListCullingProcess*)	.?AVNiCullingProcess@@
[2023-09-13 02:50:52.746] [Global] [info] [34776] [Introspection.cpp:1504] Found unhandled type:	(BSGeometryListCullingProcess*)	.?AVBSGeometryListCullingProcess@@
[2023-09-13 02:50:52.746] [Global] [info] [34776] [Introspection.cpp:1504] Found unhandled type:	(BSGeometryListCullingProcess*)	.?AVBSCullingProcess@@
[2023-09-13 02:50:52.746] [Global] [info] [34776] [Introspection.cpp:1504] Found unhandled type:	(BSGeometryListCullingProcess*)	.?AVNiCullingProcess@@
[2023-09-13 02:50:52.746] [Global] [info] [24832] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+0DA440F	Unable to locate PDB
[2023-09-13 02:50:52.746] [Global] [info] [24832] [Introspection.cpp:1504] Found unhandled type:	(BSFadeNode*)	.?AVBSFadeNode@@
[2023-09-13 02:50:52.746] [Global] [info] [24832] [Introspection.cpp:1504] Found unhandled type:	(BSFadeNode*)	.?AVNiNode@@
[2023-09-13 02:50:52.746] [Global] [info] [24832] [Introspection.cpp:1504] Found unhandled type:	(BSFadeNode*)	.?AVNiObject@@
[2023-09-13 02:50:52.746] [Global] [info] [24832] [Introspection.cpp:1504] Found unhandled type:	(BSFadeNode*)	.?AVNiRefObject@@
[2023-09-13 02:50:52.746] [Global] [info] [26712] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+2FEE2A0 with path Data/SKSE/Plugins
[2023-09-13 02:50:52.746] [Global] [info] [26712] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+2FEE2A0	Unable to locate PDB
[2023-09-13 02:50:52.746] [Global] [info] [24832] [Introspection.cpp:1504] Found unhandled type:	(BShkbAnimationGraph*)	.?AVBSIRagdollDriver@@
[2023-09-13 02:50:52.746] [Global] [info] [24832] [Introspection.cpp:1504] Found unhandled type:	(BShkbAnimationGraph*)	.?AUBSIntrusiveRefCounted@@
[2023-09-13 02:50:52.746] [Global] [info] [24832] [Introspection.cpp:1504] Found unhandled type:	(BShkbAnimationGraph*)	.?AV?$BSTEventSource@VBSTransformDeltaEvent@@@@
[2023-09-13 02:50:52.746] [Global] [info] [32724] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+0B9F79D with path Data/SKSE/Plugins
[2023-09-13 02:50:52.746] [Global] [info] [24832] [Introspection.cpp:1504] Found unhandled type:	(BShkbAnimationGraph*)	.?AV?$BSTEventSource@UBSAnimationGraphEvent@@@@
[2023-09-13 02:50:52.746] [Global] [info] [26712] [Introspection.cpp:1504] Found unhandled type:	(BShkbAnimationGraph*)	.?AVBSIRagdollDriver@@
[2023-09-13 02:50:52.746] [Global] [info] [26712] [Introspection.cpp:1504] Found unhandled type:	(BShkbAnimationGraph*)	.?AUBSIntrusiveRefCounted@@
[2023-09-13 02:50:52.746] [Global] [info] [26712] [Introspection.cpp:1504] Found unhandled type:	(BShkbAnimationGraph*)	.?AV?$BSTEventSource@VBSTransformDeltaEvent@@@@
[2023-09-13 02:50:52.746] [Global] [info] [26712] [Introspection.cpp:1504] Found unhandled type:	(BShkbAnimationGraph*)	.?AV?$BSTEventSource@UBSAnimationGraphEvent@@@@
[2023-09-13 02:50:52.746] [Global] [info] [32724] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+0B9F79D	Unable to locate PDB
[2023-09-13 02:50:52.747] [Global] [info] [30372] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+038D29D with path Data/SKSE/Plugins
[2023-09-13 02:50:52.747] [Global] [info] [30372] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+038D29D	Unable to locate PDB
[2023-09-13 02:50:52.747] [Global] [info] [30372] [Introspection.cpp:1504] Found unhandled type:	(ahkpWorld*)	.?AVahkpWorld@@
[2023-09-13 02:50:52.747] [Global] [info] [30372] [Introspection.cpp:1504] Found unhandled type:	(ahkpWorld*)	.?AVhkpWorld@@
[2023-09-13 02:50:52.747] [Global] [info] [30372] [Introspection.cpp:1504] Found unhandled type:	(ahkpWorld*)	.?AVhkReferencedObject@@
[2023-09-13 02:50:52.747] [Global] [info] [30372] [Introspection.cpp:1504] Found unhandled type:	(ahkpWorld*)	.?AVhkBaseObject@@
[2023-09-13 02:50:52.747] [Global] [info] [33280] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+033CC8F with path Data/SKSE/Plugins
[2023-09-13 02:50:52.747] [Global] [info] [33280] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+033CC8F	Unable to locate PDB
[2023-09-13 02:50:52.747] [Global] [info] [34404] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+0A9D4F5 with path Data/SKSE/Plugins
[2023-09-13 02:50:52.747] [Global] [info] [34404] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+0A9D4F5	Unable to locate PDB
[2023-09-13 02:50:52.747] [Global] [info] [26680] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/tbbmalloc.dll+00157C3 with path Data/SKSE/Plugins
[2023-09-13 02:50:52.748] [Global] [info] [34548] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+2FEA3A0 with path Data/SKSE/Plugins
[2023-09-13 02:50:52.748] [Global] [info] [34548] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+2FEA3A0	Unable to locate PDB
[2023-09-13 02:50:52.748] [Global] [info] [32688] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+04EEFA3 with path Data/SKSE/Plugins
[2023-09-13 02:50:52.748] [Global] [info] [32688] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+04EEFA3	Unable to locate PDB
[2023-09-13 02:50:52.748] [Global] [info] [23216] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+04EF95C with path Data/SKSE/Plugins
[2023-09-13 02:50:52.748] [Global] [info] [23216] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+04EF95C	Unable to locate PDB
[2023-09-13 02:50:52.748] [Global] [info] [18508] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+135FB7B with path Data/SKSE/Plugins
[2023-09-13 02:50:52.749] [Global] [info] [18508] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+135FB7B	Unable to locate PDB
[2023-09-13 02:50:52.749] [Global] [info] [26996] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+161A598 with path Data/SKSE/Plugins
[2023-09-13 02:50:52.749] [Global] [info] [32404] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/tbbmalloc.dll+0013911	Unable to locate PDB
[2023-09-13 02:50:52.749] [Global] [info] [26680] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/tbbmalloc.dll+00157C3	Unable to locate PDB
[2023-09-13 02:50:52.749] [Global] [info] [29936] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/tbbmalloc.dll+00157C3	Unable to locate PDB
[2023-09-13 02:50:52.749] [Global] [info] [26996] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+161A598	Unable to locate PDB
[2023-09-13 02:50:52.749] [Global] [info] [26680] [Introspection.cpp:1504] Found unhandled type:	(BGSStoryTeller*)	.?AVBGSStoryTeller@@
[2023-09-13 02:50:52.749] [Global] [info] [26680] [Introspection.cpp:1504] Found unhandled type:	(BGSStoryTeller*)	.?AU?$BSTSingletonSDM@VBGSStoryTeller@@UBSTSingletonSDMOpStaticBuffer@@@@
[2023-09-13 02:50:52.749] [Global] [info] [26680] [Introspection.cpp:1504] Found unhandled type:	(BGSStoryTeller*)	.?AU?$BSTSingletonSDMBase@U?$BSTSDMTraits@VBGSStoryTeller@@U?$BSTSingletonSDMOpStaticBuffer@VBGSStoryTeller@@@@@@@@
[2023-09-13 02:50:52.749] [Global] [info] [26680] [Introspection.cpp:1504] Found unhandled type:	(BGSStoryTeller*)	.?AU?$BSTSDMTraits@VBGSStoryTeller@@U?$BSTSingletonSDMOpStaticBuffer@VBGSStoryTeller@@@@@@
[2023-09-13 02:50:52.749] [Global] [info] [26680] [Introspection.cpp:1504] Found unhandled type:	(BGSStoryTeller*)	.?AU?$BSTSingletonSDMOpStaticBuffer@VBGSStoryTeller@@@@
[2023-09-13 02:50:52.749] [Global] [info] [26680] [Introspection.cpp:1504] Found unhandled type:	(BGSStoryTeller*)	.?AV?$BSTEventSink@UTESQuestStageItemDoneEvent@@@@
[2023-09-13 02:50:52.749] [Global] [info] [31288] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+13A3021 with path Data/SKSE/Plugins
[2023-09-13 02:50:52.749] [Global] [info] [29936] [Introspection.cpp:1504] Found unhandled type:	(ScrapHeap*)	.?AVScrapHeap@@
[2023-09-13 02:50:52.749] [Global] [info] [29936] [Introspection.cpp:1504] Found unhandled type:	(ScrapHeap*)	.?AVIMemoryStore@@
[2023-09-13 02:50:52.749] [Global] [info] [29936] [Introspection.cpp:1504] Found unhandled type:	(ScrapHeap*)	.?AVIMemoryStoreBase@@
[2023-09-13 02:50:52.749] [Global] [info] [29936] [Introspection.cpp:1504] Found unhandled type:	(BSGeometryListCullingProcess*)	.?AVBSGeometryListCullingProcess@@
[2023-09-13 02:50:52.749] [Global] [info] [29936] [Introspection.cpp:1504] Found unhandled type:	(BSGeometryListCullingProcess*)	.?AVBSCullingProcess@@
[2023-09-13 02:50:52.749] [Global] [info] [29936] [Introspection.cpp:1504] Found unhandled type:	(BSGeometryListCullingProcess*)	.?AVNiCullingProcess@@
[2023-09-13 02:50:52.749] [Global] [info] [31288] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+13A3021	Unable to locate PDB
[2023-09-13 02:50:52.749] [Global] [info] [31288] [Introspection.cpp:1504] Found unhandled type:	(BSGeometryListCullingProcess*)	.?AVBSGeometryListCullingProcess@@
[2023-09-13 02:50:52.749] [Global] [info] [31288] [Introspection.cpp:1504] Found unhandled type:	(BSGeometryListCullingProcess*)	.?AVBSCullingProcess@@
[2023-09-13 02:50:52.749] [Global] [info] [31288] [Introspection.cpp:1504] Found unhandled type:	(BSGeometryListCullingProcess*)	.?AVNiCullingProcess@@
[2023-09-13 02:50:52.749] [Global] [info] [31288] [Introspection.cpp:1504] Found unhandled type:	(BSGeometryListCullingProcess*)	.?AVBSGeometryListCullingProcess@@
[2023-09-13 02:50:52.749] [Global] [info] [31288] [Introspection.cpp:1504] Found unhandled type:	(BSGeometryListCullingProcess*)	.?AVBSCullingProcess@@
[2023-09-13 02:50:52.749] [Global] [info] [31288] [Introspection.cpp:1504] Found unhandled type:	(BSGeometryListCullingProcess*)	.?AVNiCullingProcess@@
[2023-09-13 02:50:52.749] [Global] [info] [31288] [Introspection.cpp:1504] Found unhandled type:	(BSMultiBoundNode*)	.?AVBSMultiBoundNode@@
[2023-09-13 02:50:52.749] [Global] [info] [31288] [Introspection.cpp:1504] Found unhandled type:	(BSMultiBoundNode*)	.?AVBSNiNode@@
[2023-09-13 02:50:52.749] [Global] [info] [31288] [Introspection.cpp:1504] Found unhandled type:	(BSMultiBoundNode*)	.?AVNiNode@@
[2023-09-13 02:50:52.749] [Global] [info] [31288] [Introspection.cpp:1504] Found unhandled type:	(BSMultiBoundNode*)	.?AVNiObject@@
[2023-09-13 02:50:52.749] [Global] [info] [31288] [Introspection.cpp:1504] Found unhandled type:	(BSMultiBoundNode*)	.?AVNiRefObject@@
[2023-09-13 02:50:52.749] [Global] [info] [31884] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+0CAC998 with path Data/SKSE/Plugins
[2023-09-13 02:50:52.750] [Global] [info] [31884] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+0CAC998	Unable to locate PDB
[2023-09-13 02:50:52.750] [Global] [info] [33644] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+0DA440F with path Data/SKSE/Plugins
[2023-09-13 02:50:52.750] [Global] [info] [33644] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+0DA440F	Unable to locate PDB
[2023-09-13 02:50:52.750] [Global] [info] [34580] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+04EECB6 with path Data/SKSE/Plugins
[2023-09-13 02:50:52.750] [Global] [info] [34580] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+04EECB6	Unable to locate PDB
[2023-09-13 02:50:52.750] [Global] [info] [34580] [Introspection.cpp:1504] Found unhandled type:	(BGSStoryTeller*)	.?AVBGSStoryTeller@@
[2023-09-13 02:50:52.750] [Global] [info] [34580] [Introspection.cpp:1504] Found unhandled type:	(BGSStoryTeller*)	.?AU?$BSTSingletonSDM@VBGSStoryTeller@@UBSTSingletonSDMOpStaticBuffer@@@@
[2023-09-13 02:50:52.750] [Global] [info] [34580] [Introspection.cpp:1504] Found unhandled type:	(BGSStoryTeller*)	.?AU?$BSTSingletonSDMBase@U?$BSTSDMTraits@VBGSStoryTeller@@U?$BSTSingletonSDMOpStaticBuffer@VBGSStoryTeller@@@@@@@@
[2023-09-13 02:50:52.750] [Global] [info] [34580] [Introspection.cpp:1504] Found unhandled type:	(BGSStoryTeller*)	.?AU?$BSTSDMTraits@VBGSStoryTeller@@U?$BSTSingletonSDMOpStaticBuffer@VBGSStoryTeller@@@@@@
[2023-09-13 02:50:52.750] [Global] [info] [34580] [Introspection.cpp:1504] Found unhandled type:	(BGSStoryTeller*)	.?AU?$BSTSingletonSDMOpStaticBuffer@VBGSStoryTeller@@@@
[2023-09-13 02:50:52.750] [Global] [info] [34580] [Introspection.cpp:1504] Found unhandled type:	(BGSStoryTeller*)	.?AV?$BSTEventSink@UTESQuestStageItemDoneEvent@@@@
[2023-09-13 02:50:52.750] [Global] [info] [34524] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+0A9FC4F with path Data/SKSE/Plugins
[2023-09-13 02:50:52.751] [Global] [info] [34524] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+0A9FC4F	Unable to locate PDB
[2023-09-13 02:50:52.751] [Global] [info] [34556] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+04EECB6 with path Data/SKSE/Plugins
[2023-09-13 02:50:52.751] [Global] [info] [34556] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+04EECB6	Unable to locate PDB
[2023-09-13 02:50:52.751] [Global] [info] [29940] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+0AA2D24 with path Data/SKSE/Plugins
[2023-09-13 02:50:52.751] [Global] [info] [29940] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+0AA2D24	Unable to locate PDB
[2023-09-13 02:50:52.751] [Global] [info] [26008] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+07271AF with path Data/SKSE/Plugins
[2023-09-13 02:50:52.751] [Global] [info] [26008] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+07271AF	Unable to locate PDB
[2023-09-13 02:50:52.751] [Global] [info] [34532] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+0E021C8 with path Data/SKSE/Plugins
[2023-09-13 02:50:52.752] [Global] [info] [34532] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+0E021C8	Unable to locate PDB
[2023-09-13 02:50:52.752] [Global] [info] [34560] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+0C3E93F with path Data/SKSE/Plugins
[2023-09-13 02:50:52.752] [Global] [info] [34560] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+0C3E93F	Unable to locate PDB
[2023-09-13 02:50:52.752] [Global] [info] [34456] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+04EECB6 with path Data/SKSE/Plugins
[2023-09-13 02:50:52.752] [Global] [info] [34456] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+04EECB6	Unable to locate PDB
[2023-09-13 02:50:52.752] [Global] [info] [28840] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+2FECE60 with path Data/SKSE/Plugins
[2023-09-13 02:50:52.752] [Global] [info] [28840] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+2FECE60	Unable to locate PDB
[2023-09-13 02:50:52.753] [Global] [info] [28840] [Introspection.cpp:1504] Found unhandled type:	(BSJobs::JobThread*)	.?AVJobThread@BSJobs@@
[2023-09-13 02:50:52.753] [Global] [info] [28840] [Introspection.cpp:1504] Found unhandled type:	(BSJobs::JobThread*)	.?AVBSThread@@
[2023-09-13 02:50:52.753] [Global] [info] [5640] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+04ECB11 with path Data/SKSE/Plugins
[2023-09-13 02:50:52.753] [Global] [info] [5640] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+04ECB11	Unable to locate PDB
[2023-09-13 02:50:52.753] [Global] [info] [34552] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+01560EE with path Data/SKSE/Plugins
[2023-09-13 02:50:52.753] [Global] [info] [34552] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+01560EE	Unable to locate PDB
[2023-09-13 02:50:52.753] [Global] [info] [34544] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+0D7F8A8 with path Data/SKSE/Plugins
[2023-09-13 02:50:52.753] [Global] [info] [34544] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+0D7F8A8	Unable to locate PDB
[2023-09-13 02:50:52.753] [Global] [info] [17392] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+0DA440F with path Data/SKSE/Plugins
[2023-09-13 02:50:52.754] [Global] [info] [17392] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+0DA440F	Unable to locate PDB
[2023-09-13 02:50:52.754] [Global] [info] [34280] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+161A598 with path Data/SKSE/Plugins
[2023-09-13 02:50:52.754] [Global] [info] [34280] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+161A598	Unable to locate PDB
[2023-09-13 02:50:52.754] [Global] [info] [34476] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+0CAC998 with path Data/SKSE/Plugins
[2023-09-13 02:50:52.754] [Global] [info] [34280] [Introspection.cpp:1504] Found unhandled type:	(BSJobs::JobThread*)	.?AVJobThread@BSJobs@@
[2023-09-13 02:50:52.754] [Global] [info] [34280] [Introspection.cpp:1504] Found unhandled type:	(BSJobs::JobThread*)	.?AVBSThread@@
[2023-09-13 02:50:52.754] [Global] [info] [34476] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+0CAC998	Unable to locate PDB
[2023-09-13 02:50:52.754] [Global] [info] [29412] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+0D9C421 with path Data/SKSE/Plugins
[2023-09-13 02:50:52.755] [Global] [info] [29412] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+0D9C421	Unable to locate PDB
[2023-09-13 02:50:52.755] [Global] [info] [30192] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+0390875 with path Data/SKSE/Plugins
[2023-09-13 02:50:52.755] [Global] [info] [29412] [Introspection.cpp:1504] Found unhandled type:	(BSJobs::JobThread*)	.?AVJobThread@BSJobs@@
[2023-09-13 02:50:52.755] [Global] [info] [29412] [Introspection.cpp:1504] Found unhandled type:	(BSJobs::JobThread*)	.?AVBSThread@@
[2023-09-13 02:50:52.755] [Global] [info] [30192] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+0390875	Unable to locate PDB
[2023-09-13 02:50:52.755] [Global] [info] [34528] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+0B2C4C2 with path Data/SKSE/Plugins
[2023-09-13 02:50:52.755] [Global] [info] [34528] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+0B2C4C2	Unable to locate PDB
[2023-09-13 02:50:52.755] [Global] [info] [34528] [Introspection.cpp:1504] Found unhandled type:	(BSJobs::JobThread*)	.?AVJobThread@BSJobs@@
[2023-09-13 02:50:52.755] [Global] [info] [34528] [Introspection.cpp:1504] Found unhandled type:	(BSJobs::JobThread*)	.?AVBSThread@@
[2023-09-13 02:50:52.755] [Global] [info] [34528] [Introspection.cpp:1504] Found unhandled type:	(BSJobs::JobThread*)	.?AVJobThread@BSJobs@@
[2023-09-13 02:50:52.755] [Global] [info] [34528] [Introspection.cpp:1504] Found unhandled type:	(BSJobs::JobThread*)	.?AVBSThread@@
[2023-09-13 02:50:52.755] [Global] [info] [33444] [PdbHandler.cpp:189] Attempting to find pdb for C:/WINDOWS/System32/ucrtbase.dll+0038848 with path Data/SKSE/Plugins
[2023-09-13 02:50:52.755] [Global] [info] [29804] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+050E59E with path Data/SKSE/Plugins
[2023-09-13 02:50:52.756] [Global] [info] [29804] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+050E59E	Unable to locate PDB
[2023-09-13 02:50:52.756] [Global] [info] [31588] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+064B48B with path Data/SKSE/Plugins
[2023-09-13 02:50:52.756] [Global] [info] [33444] [PdbHandler.cpp:193] Failed to open pdb for dll C:/WINDOWS/System32/ucrtbase.dll+0038848	Unable to locate PDB
[2023-09-13 02:50:52.756] [Global] [info] [31588] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+064B48B	Unable to locate PDB
[2023-09-13 02:50:52.756] [Global] [info] [26984] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+061B381 with path Data/SKSE/Plugins
[2023-09-13 02:50:52.756] [Global] [info] [26984] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+061B381	Unable to locate PDB
[2023-09-13 02:50:52.756] [Global] [info] [34344] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+064543D with path Data/SKSE/Plugins
[2023-09-13 02:50:52.757] [Global] [info] [34344] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+064543D	Unable to locate PDB
[2023-09-13 02:50:52.757] [Global] [info] [34584] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+0A004BE with path Data/SKSE/Plugins
[2023-09-13 02:50:52.757] [Global] [info] [34584] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+0A004BE	Unable to locate PDB
[2023-09-13 02:50:52.757] [Global] [info] [27660] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+13B46F0 with path Data/SKSE/Plugins
[2023-09-13 02:50:52.757] [Global] [info] [27660] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+13B46F0	Unable to locate PDB
[2023-09-13 02:50:52.757] [Global] [info] [32488] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+13B438C with path Data/SKSE/Plugins
[2023-09-13 02:50:52.757] [Global] [info] [32488] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+13B438C	Unable to locate PDB
[2023-09-13 02:50:52.757] [Global] [info] [28656] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+13B46F0 with path Data/SKSE/Plugins
[2023-09-13 02:50:52.758] [Global] [info] [28656] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+13B46F0	Unable to locate PDB
[2023-09-13 02:50:52.758] [Global] [info] [25836] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+0B24B4E with path Data/SKSE/Plugins
[2023-09-13 02:50:52.758] [Global] [info] [25836] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+0B24B4E	Unable to locate PDB
[2023-09-13 02:50:52.758] [Global] [info] [34768] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+0C92D3B with path Data/SKSE/Plugins
[2023-09-13 02:50:52.758] [Global] [info] [34768] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+0C92D3B	Unable to locate PDB
[2023-09-13 02:50:52.758] [Global] [info] [34460] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+13B4326 with path Data/SKSE/Plugins
[2023-09-13 02:50:52.758] [Global] [info] [34460] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+13B4326	Unable to locate PDB
[2023-09-13 02:50:52.759] [Global] [info] [34776] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+0D9C421 with path Data/SKSE/Plugins
[2023-09-13 02:50:52.759] [Global] [info] [34776] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+0D9C421	Unable to locate PDB
[2023-09-13 02:50:52.759] [Global] [info] [24832] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+0B25B63 with path Data/SKSE/Plugins
[2023-09-13 02:50:52.759] [Global] [info] [24832] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+0B25B63	Unable to locate PDB
[2023-09-13 02:50:52.759] [Global] [info] [26712] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/tbbmalloc.dll+00157C3 with path Data/SKSE/Plugins
[2023-09-13 02:50:52.759] [Global] [info] [26712] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/tbbmalloc.dll+00157C3	Unable to locate PDB
[2023-09-13 02:50:52.759] [Global] [info] [32724] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/tbbmalloc.dll+00157C3 with path Data/SKSE/Plugins
[2023-09-13 02:50:52.760] [Global] [info] [32724] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/tbbmalloc.dll+00157C3	Unable to locate PDB
[2023-09-13 02:50:52.760] [Global] [info] [30372] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+1165454 with path Data/SKSE/Plugins
[2023-09-13 02:50:52.760] [Global] [info] [30372] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+1165454	Unable to locate PDB
[2023-09-13 02:50:52.760] [Global] [info] [33280] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+3092644 with path Data/SKSE/Plugins
[2023-09-13 02:50:52.760] [Global] [info] [33280] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+3092644	Unable to locate PDB
[2023-09-13 02:50:52.760] [Global] [info] [34404] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/tbbmalloc.dll+00383C0 with path Data/SKSE/Plugins
[2023-09-13 02:50:52.760] [Global] [info] [34404] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/tbbmalloc.dll+00383C0	Unable to locate PDB
[2023-09-13 02:50:52.760] [Global] [info] [34548] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+135FBFD with path Data/SKSE/Plugins
[2023-09-13 02:50:52.761] [Global] [info] [34548] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+135FBFD	Unable to locate PDB
[2023-09-13 02:50:52.761] [Global] [info] [32688] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/tbbmalloc.dll+0017A16 with path Data/SKSE/Plugins
[2023-09-13 02:50:52.761] [Global] [info] [32688] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/tbbmalloc.dll+0017A16	Unable to locate PDB
[2023-09-13 02:50:52.761] [Global] [info] [23216] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+0B23C8E with path Data/SKSE/Plugins
[2023-09-13 02:50:52.761] [Global] [info] [23216] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+0B23C8E	Unable to locate PDB
[2023-09-13 02:50:52.761] [Global] [info] [18508] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+3092644 with path Data/SKSE/Plugins
[2023-09-13 02:50:52.761] [Global] [info] [18508] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+3092644	Unable to locate PDB
[2023-09-13 02:50:52.762] [Global] [info] [32404] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+04F2DE0 with path Data/SKSE/Plugins
[2023-09-13 02:50:52.762] [Global] [info] [32404] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+04F2DE0	Unable to locate PDB
[2023-09-13 02:50:52.762] [Global] [info] [26996] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+161A2B8 with path Data/SKSE/Plugins
[2023-09-13 02:50:52.762] [Global] [info] [26996] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+161A2B8	Unable to locate PDB
[2023-09-13 02:50:52.762] [Global] [info] [26680] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+0CB47EC with path Data/SKSE/Plugins
[2023-09-13 02:50:52.762] [Global] [info] [26680] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+0CB47EC	Unable to locate PDB
[2023-09-13 02:50:52.762] [Global] [info] [29936] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+0D9C6E1 with path Data/SKSE/Plugins
[2023-09-13 02:50:52.763] [Global] [info] [29936] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+0D9C6E1	Unable to locate PDB
[2023-09-13 02:50:52.763] [Global] [info] [31288] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+3092644 with path Data/SKSE/Plugins
[2023-09-13 02:50:52.763] [Global] [info] [31288] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+3092644	Unable to locate PDB
[2023-09-13 02:50:52.763] [Global] [info] [31884] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+3092640 with path Data/SKSE/Plugins
[2023-09-13 02:50:52.763] [Global] [info] [31884] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+3092640	Unable to locate PDB
[2023-09-13 02:50:52.763] [Global] [info] [33644] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+3092648 with path Data/SKSE/Plugins
[2023-09-13 02:50:52.763] [Global] [info] [33644] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+3092648	Unable to locate PDB
[2023-09-13 02:50:52.763] [Global] [info] [34580] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+04F2A45 with path Data/SKSE/Plugins
[2023-09-13 02:50:52.764] [Global] [info] [34580] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+04F2A45	Unable to locate PDB
[2023-09-13 02:50:52.764] [Global] [info] [34524] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+0678A56 with path Data/SKSE/Plugins
[2023-09-13 02:50:52.764] [Global] [info] [34524] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+0678A56	Unable to locate PDB
[2023-09-13 02:50:52.764] [Global] [info] [34556] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+14062CE with path Data/SKSE/Plugins
[2023-09-13 02:50:52.764] [Global] [info] [34556] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+14062CE	Unable to locate PDB
[2023-09-13 02:50:52.764] [Global] [info] [29940] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+3092644 with path Data/SKSE/Plugins
[2023-09-13 02:50:52.765] [Global] [info] [29940] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+3092644	Unable to locate PDB
[2023-09-13 02:50:52.765] [Global] [info] [26008] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+30950E0 with path Data/SKSE/Plugins
[2023-09-13 02:50:52.765] [Global] [info] [26008] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+30950E0	Unable to locate PDB
[2023-09-13 02:50:52.765] [Global] [info] [34532] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+0C6C628 with path Data/SKSE/Plugins
[2023-09-13 02:50:52.765] [Global] [info] [34532] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+0C6C628	Unable to locate PDB
[2023-09-13 02:50:52.765] [Global] [info] [34560] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+30950E0 with path Data/SKSE/Plugins
[2023-09-13 02:50:52.765] [Global] [info] [34560] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+30950E0	Unable to locate PDB
[2023-09-13 02:50:52.765] [Global] [info] [34456] [PdbHandler.cpp:189] Attempting to find pdb for C:/WINDOWS/System32/KERNELBASE.dll+00670CD with path Data/SKSE/Plugins
[2023-09-13 02:50:52.766] [Global] [info] [28840] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+3095090 with path Data/SKSE/Plugins
[2023-09-13 02:50:52.766] [Global] [info] [28840] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+3095090	Unable to locate PDB
[2023-09-13 02:50:52.766] [Global] [info] [34456] [PdbHandler.cpp:193] Failed to open pdb for dll C:/WINDOWS/System32/KERNELBASE.dll+00670CD	Unable to locate PDB
[2023-09-13 02:50:52.766] [Global] [info] [5640] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+30A8300 with path Data/SKSE/Plugins
[2023-09-13 02:50:52.766] [Global] [info] [5640] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+30A8300	Unable to locate PDB
[2023-09-13 02:50:52.766] [Global] [info] [34552] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+0C6CBF1 with path Data/SKSE/Plugins
[2023-09-13 02:50:52.766] [Global] [info] [34552] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+0C6CBF1	Unable to locate PDB
[2023-09-13 02:50:52.766] [Global] [info] [34544] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/Data/SKSE/Plugins/EngineFixes.dll+0015D19 with path Data/SKSE/Plugins
[2023-09-13 02:50:52.767] [Global] [info] [17392] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+1F56F80 with path Data/SKSE/Plugins
[2023-09-13 02:50:52.767] [Global] [info] [17392] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+1F56F80	Unable to locate PDB
[2023-09-13 02:50:52.767] [Global] [info] [34280] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+0C6AF7A with path Data/SKSE/Plugins
[2023-09-13 02:50:52.767] [Global] [info] [34280] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+0C6AF7A	Unable to locate PDB
[2023-09-13 02:50:52.767] [Global] [info] [34476] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+3095001 with path Data/SKSE/Plugins
[2023-09-13 02:50:52.768] [Global] [info] [34476] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+3095001	Unable to locate PDB
[2023-09-13 02:50:52.768] [Global] [info] [29412] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+0C45E4D with path Data/SKSE/Plugins
[2023-09-13 02:50:52.768] [Global] [info] [29412] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+0C45E4D	Unable to locate PDB
[2023-09-13 02:50:52.768] [Global] [info] [30192] [PdbHandler.cpp:189] Attempting to find pdb for D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+30068F0 with path Data/SKSE/Plugins
[2023-09-13 02:50:52.768] [Global] [info] [30192] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/SkyrimSE.exe+30068F0	Unable to locate PDB
[2023-09-13 02:50:52.768] [Global] [info] [34528] [PdbHandler.cpp:189] Attempting to find pdb for C:/WINDOWS/System32/KERNEL32.DLL+00126AD with path Data/SKSE/Plugins
[2023-09-13 02:50:52.768] [Global] [info] [34528] [PdbHandler.cpp:193] Failed to open pdb for dll C:/WINDOWS/System32/KERNEL32.DLL+00126AD	Unable to locate PDB
[2023-09-13 02:50:52.768] [Global] [info] [29804] [PdbHandler.cpp:189] Attempting to find pdb for C:/WINDOWS/SYSTEM32/ntdll.dll+005AA68 with path Data/SKSE/Plugins
[2023-09-13 02:50:52.769] [Global] [info] [29804] [PdbHandler.cpp:193] Failed to open pdb for dll C:/WINDOWS/SYSTEM32/ntdll.dll+005AA68	Unable to locate PDB
[2023-09-13 02:50:52.769] [Global] [info] [31588] [PdbHandler.cpp:189] Attempting to find pdb for C:/WINDOWS/System32/KERNELBASE.dll+015BD30 with path Data/SKSE/Plugins
[2023-09-13 02:50:52.769] [Global] [info] [31588] [PdbHandler.cpp:193] Failed to open pdb for dll C:/WINDOWS/System32/KERNELBASE.dll+015BD30	Unable to locate PDB
[2023-09-13 02:50:52.784] [Global] [info] [34544] [PdbHandler.cpp:193] Failed to open pdb for dll D:/SteamLibrary/steamapps/common/Skyrim Special Edition/Data/SKSE/Plugins/EngineFixes.dll+0015D19	Unable to locate PDB


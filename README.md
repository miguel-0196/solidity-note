- bytes("") = 0x

- address(proxy).staticcall(hex"5c60da1b")

- bytes4  U2D_FUNC_SIG = bytes4(keccak256("upgradeToAndCall(address,bytes)"));

- abi.encodeWithSelector(U2D_FUNC_SIG, newImpl, data)

- target.delegatecall(abi.encodeWithSelector(bytes4(keccak256("initialize()"))));

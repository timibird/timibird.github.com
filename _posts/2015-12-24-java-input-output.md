---
layout: post
title: JAVA Input/Output
---
**JAVA 입출력**

0. Stream
Stream : Byte 단위

1. InputStream
InputStream : abstract Interface

2. OutputStream
OutputStream : abstract Interface

3. Example
3-1. (return int) System.in.read() : 아스키코드 하나의 값을 받는다.
		int value;
		value = System.in.read();		//input A
		System.out.println(value);		//output 65
		System.out.println((char)value);	//output A
	형변환을 통해 아스키코드를 출력할 수 있다. 한 번에 하나의 값을 받아 출력하므로, 다중의 값이 입력될 때 다음과 같은 문제가 있다.
		int a, b, c, d;
		//input A, B
		a = System.in.read();
		b = System.in.read();
		c = System.in.read();
		d = System.in.read();

		Sysetm.out.println(a);	//output 65(A)
		Sysetm.out.println(b);	//output 13
		Sysetm.out.println(c);	//output 10
		Sysetm.out.println(d);	//output 66(B)

	Enter : 개행문자(\r\n)
	output 13 is \r			//캐럿이 그줄 맨 앞으로(Carriage Return)
	output 10 is \n			//캐럿이 다음 줄로(Line Feed)

3-2. (return String) BufferedReader(new InputStreamReader(System.in)) : 개행되기 전까지 모든 문자열을 받는다.
	BufferedReader in = new BufferedReader(new InputStreamReader(System.in));
	String a, b;
	a = in.readLine();			//input TEST
	b = in.readLine();			//input HELLO WORLD
	System.out.println(a);		//output TEST
	System.out.println(b);		//output HELLO woRLD





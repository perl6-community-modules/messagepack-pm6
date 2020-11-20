# MessagePack

MessagePack は [MessagePack](http://msgpack.org/) の Raku 実装です。

MessagePack の作成にあたっては以下のライブラリを参考にしています：

  - MessagePack-JS http://github.com/cuzic/MessagePack-JS
  - msgpack_pure   http://github.com/nayutaya/msgpack-pure

MessagePack is a Raku implementation of
[MessagePack](http://msgpack.org/).

We refered to the following library when creating MessagePack.pm6:

  - MessagePack-JS http://github.com/cuzic/MessagePack-JS
  - msgpack_pure   http://github.com/nayutaya/msgpack-pure

## Synopsis

    use MessagePack;

    my $unpacker = MessagePack::Unpacker;
    my $buffer = buf8.new(0x93, 0x01, 0x02, 0x03);
    say $unpacker.unpack($buffer);  # (1 2 3)

## Author

Originally written by:

    - Tomoki Aonuma <uasi@99cm.org>

Now maintained by the Raku Community.

## Copyright

2010-2011 Tomoki Aonuma <uasi@99cm.org>

2014-2016 The Raku Community

## See also

  - http://msgpack.org/ - MessagePack serialization format

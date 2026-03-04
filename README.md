Лабараторная работа №1  Автор: Меликов Гарик, Группа: ИУ8-23


1. Скачайте библиотеку *boost* с помощью утилиты **wget**. Адрес для скачивания `https://sourceforge.net/projects/boost/files/boost/1.69.0/boost_1_69_0.tar.gz`.
Решение: wget https://sourceforge.net/projects/boost/files/boost/1.90.0/boost_1_90_0.tar.gz

Вывод: --2026-03-04 10:20:39--  https://sourceforge.net/projects/boost/files/boost/1.90.0/boost_1_90_0.tar.gz
Resolving sourceforge.net (sourceforge.net)... 104.18.12.149, 104.18.13.149, 2606:4700::6812:c95, ...
Connecting to sourceforge.net (sourceforge.net)|104.18.12.149|:443... connected.
HTTP request sent, awaiting response... 301 Moved Permanently
Location: https://sourceforge.net/projects/boost/files/boost/1.90.0/boost_1_90_0.tar.gz/ [following]
--2026-03-04 10:20:40--  https://sourceforge.net/projects/boost/files/boost/1.90.0/boost_1_90_0.tar.gz/
Reusing existing connection to sourceforge.net:443.
HTTP request sent, awaiting response... 301 Moved Permanently
Location: https://sourceforge.net/projects/boost/files/boost/1.90.0/boost_1_90_0.tar.gz/download [following]
--2026-03-04 10:20:41--  https://sourceforge.net/projects/boost/files/boost/1.90.0/boost_1_90_0.tar.gz/download
Reusing existing connection to sourceforge.net:443.
HTTP request sent, awaiting response... 302 Found
Location: https://downloads.sourceforge.net/project/boost/boost/1.90.0/boost_1_90_0.tar.gz?ts=gAAAAABpqFu0Iwwyko-eT1GxP3ysl0OUZmoChXNDRq9bwyHg91_Vn_sKaJXjcMmjWOtowrVAC2QtuOzBkV>
--2026-03-04 10:20:41--  https://downloads.sourceforge.net/project/boost/boost/1.90.0/boost_1_90_0.tar.gz?ts=gAAAAABpqFu0Iwwyko-eT1GxP3ysl0OUZmoChXNDRq9bwyHg91_Vn_sKaJXjcMmjWOt>
Resolving downloads.sourceforge.net (downloads.sourceforge.net)... 104.18.12.149, 104.18.13.149, 2606:4700::6812:d95, ...
Connecting to downloads.sourceforge.net (downloads.sourceforge.net)|104.18.12.149|:443... connected.
HTTP request sent, awaiting response... 302 Found
Location: https://deac-fra.dl.sourceforge.net/project/boost/boost/1.90.0/boost_1_90_0.tar.gz?viasf=1 [following]
--2026-03-04 10:20:42--  https://deac-fra.dl.sourceforge.net/project/boost/boost/1.90.0/boost_1_90_0.tar.gz?viasf=1
Resolving deac-fra.dl.sourceforge.net (deac-fra.dl.sourceforge.net)... 37.203.33.33
Connecting to deac-fra.dl.sourceforge.net (deac-fra.dl.sourceforge.net)|37.203.33.33|:443... connected.
HTTP request sent, awaiting response... 200 OK
Length: 210975925 (201M) [application/x-gzip]
Saving to: ‘boost_1_90_0.tar.gz.1’

boost_1_90_0.tar.gz.1                        100%[===========================================================================================>] 201.20M  4.25MB/s    in 76s     

2026-03-04 10:22:00 (2.64 MB/s) - ‘boost_1_90_0.tar.gz.1’ saved [210975925/210975925]

7. Выведите в консоль все файлы, где упоминается последовательность `boost::asio`.
Решение: grep -rl "boost::asio" ~/boost_1_90_0
Вывод:
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp03/can_prefer_not_applicable_unsupported.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp03/prefer_unsupported.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp03/require_concept_member.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp03/can_require_concept_not_applicable_member.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp03/can_require_static.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp11/can_require_not_applicable_free.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp11/require_free.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp11/can_require_concept_not_applicable_static.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp11/can_query_not_applicable_member.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp11/can_prefer_not_applicable_free_require.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp11/can_query_member.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp11/can_prefer_member_prefer.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp11/can_require_not_applicable_static.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp11/can_prefer_static.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp11/can_prefer_not_applicable_member_require.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp11/can_require_not_applicable_member.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp11/can_query_static.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp11/can_query_not_applicable_free.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp11/can_prefer_not_preferable_free_prefer.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp11/can_prefer_free_prefer.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp11/prefer_member_prefer.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp11/can_require_free.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp11/can_require_concept_static.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp11/can_prefer_not_preferable_static.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp11/can_prefer_member_require.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp11/can_require_unsupported.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp11/can_prefer_not_preferable_member_require.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp11/can_require_concept_free.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp11/can_query_not_applicable_unsupported.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp11/require_concept_static.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp11/query_static.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp11/prefer_free_prefer.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp11/can_query_free.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp11/can_prefer_unsupported.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp11/can_query_not_applicable_static.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp11/require_concept_free.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp11/can_require_member.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp11/prefer_static.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp11/can_prefer_not_preferable_free_require.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp11/can_prefer_not_applicable_member_prefer.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp11/can_require_concept_member.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp11/require_member.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp11/can_prefer_free_require.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp11/can_require_concept_not_applicable_unsupported.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp11/can_prefer_not_preferable_member_prefer.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp11/can_prefer_not_applicable_free_prefer.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp11/can_require_not_applicable_unsupported.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp11/can_prefer_not_preferable_unsupported.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp11/query_free.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp11/require_static.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp11/prefer_free_require.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp11/query_member.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp11/can_require_concept_unsupported.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp11/can_require_concept_not_applicable_free.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp11/can_prefer_not_applicable_static.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp11/prefer_member_require.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp11/can_query_unsupported.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp11/can_prefer_not_applicable_unsupported.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp11/prefer_unsupported.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp11/require_concept_member.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp11/can_require_concept_not_applicable_member.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp11/can_require_static.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp14/can_require_not_applicable_free.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp14/require_free.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp14/can_require_concept_not_applicable_static.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp14/can_query_not_applicable_member.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp14/can_prefer_not_applicable_free_require.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp14/can_query_member.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp14/can_prefer_member_prefer.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp14/can_require_not_applicable_static.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp14/can_prefer_static.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp14/can_prefer_not_applicable_member_require.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp14/can_require_not_applicable_member.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp14/can_query_static.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp14/can_query_not_applicable_free.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp14/can_prefer_not_preferable_free_prefer.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp14/can_prefer_free_prefer.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp14/prefer_member_prefer.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp14/can_require_free.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp14/can_require_concept_static.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp14/can_prefer_not_preferable_static.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp14/can_prefer_member_require.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp14/can_require_unsupported.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp14/can_prefer_not_preferable_member_require.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp14/can_require_concept_free.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp14/can_query_not_applicable_unsupported.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp14/require_concept_static.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp14/query_static.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp14/prefer_free_prefer.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp14/can_query_free.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp14/can_prefer_unsupported.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp14/can_query_not_applicable_static.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp14/require_concept_free.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp14/can_require_member.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp14/prefer_static.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp14/can_prefer_not_preferable_free_require.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp14/can_prefer_not_applicable_member_prefer.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp14/can_require_concept_member.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp14/require_member.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp14/can_prefer_free_require.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp14/can_require_concept_not_applicable_unsupported.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp14/can_prefer_not_preferable_member_prefer.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp14/can_prefer_not_applicable_free_prefer.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp14/can_require_not_applicable_unsupported.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp14/can_prefer_not_preferable_unsupported.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp14/query_free.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp14/require_static.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp14/prefer_free_require.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp14/query_member.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp14/can_require_concept_unsupported.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp14/can_require_concept_not_applicable_free.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp14/can_prefer_not_applicable_static.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp14/prefer_member_require.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp14/can_query_unsupported.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp14/can_prefer_not_applicable_unsupported.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp14/prefer_unsupported.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp14/require_concept_member.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp14/can_require_concept_not_applicable_member.cpp
/home/garik/boost_1_90_0/libs/asio/test/properties/cpp14/can_require_static.cpp
/home/garik/boost_1_90_0/libs/asio/test/stream_file.cpp
/home/garik/boost_1_90_0/libs/asio/test/generic/datagram_protocol.cpp
/home/garik/boost_1_90_0/libs/asio/test/generic/stream_protocol.cpp
/home/garik/boost_1_90_0/libs/asio/test/generic/seq_packet_protocol.cpp
/home/garik/boost_1_90_0/libs/asio/test/generic/raw_protocol.cpp
/home/garik/boost_1_90_0/libs/asio/test/inline_or_executor.cpp
/home/garik/boost_1_90_0/libs/asio/test/disposition.cpp
/home/garik/boost_1_90_0/libs/asio/doc/overview/pipes.qbk
/home/garik/boost_1_90_0/libs/asio/doc/overview/allocation.qbk
/home/garik/boost_1_90_0/libs/asio/doc/overview/buffers.qbk
/home/garik/boost_1_90_0/libs/asio/doc/overview/type_erasure.qbk
/home/garik/boost_1_90_0/libs/asio/doc/overview/coro.qbk
/home/garik/boost_1_90_0/libs/asio/doc/overview/futures.qbk
/home/garik/boost_1_90_0/libs/asio/doc/overview/channels.qbk
/home/garik/boost_1_90_0/libs/asio/doc/overview/files.qbk
/home/garik/boost_1_90_0/libs/asio/doc/overview/deferred.qbk
/home/garik/boost_1_90_0/libs/asio/doc/overview/cancellation.qbk
/home/garik/boost_1_90_0/libs/asio/doc/overview/promises.qbk
/home/garik/boost_1_90_0/libs/asio/doc/overview/parallel_group.qbk
/home/garik/boost_1_90_0/libs/asio/doc/overview/configuration.qbk
/home/garik/boost_1_90_0/libs/asio/doc/overview/spawn.qbk
/home/garik/boost_1_90_0/libs/asio/doc/overview/basics.qbk
/home/garik/boost_1_90_0/libs/asio/doc/overview/line_based.qbk
/home/garik/boost_1_90_0/libs/asio/doc/overview/signals.qbk
/home/garik/boost_1_90_0/libs/asio/doc/overview/strands.qbk
/home/garik/boost_1_90_0/libs/asio/doc/overview/token_adapters.qbk
/home/garik/boost_1_90_0/libs/asio/doc/overview/cpp20_coroutines.qbk
/home/garik/boost_1_90_0/libs/asio/doc/overview/cpp2011.qbk
/home/garik/boost_1_90_0/libs/asio/doc/overview/compose.qbk
/home/garik/boost_1_90_0/libs/asio/doc/overview/other_protocols.qbk
/home/garik/boost_1_90_0/libs/asio/doc/overview/posix.qbk
/home/garik/boost_1_90_0/libs/asio/doc/overview/ssl.qbk
/home/garik/boost_1_90_0/libs/asio/doc/overview/protocols.qbk
/home/garik/boost_1_90_0/libs/asio/doc/overview/model/completion_tokens.qbk
/home/garik/boost_1_90_0/libs/asio/doc/overview/coroutine.qbk
/home/garik/boost_1_90_0/libs/asio/doc/overview/handler_tracking.qbk
/home/garik/boost_1_90_0/libs/asio/doc/overview/immediate_completion.qbk
/home/garik/boost_1_90_0/libs/asio/doc/requirements/WaitToken.qbk
/home/garik/boost_1_90_0/libs/asio/doc/requirements/HandshakeToken.qbk
/home/garik/boost_1_90_0/libs/asio/doc/requirements/SignalToken.qbk
/home/garik/boost_1_90_0/libs/asio/doc/requirements/ResolveToken.qbk
/home/garik/boost_1_90_0/libs/asio/doc/requirements/Disposition.qbk
/home/garik/boost_1_90_0/libs/asio/doc/requirements/MutableBufferSequence.qbk
/home/garik/boost_1_90_0/libs/asio/doc/requirements/MoveAcceptToken.qbk
/home/garik/boost_1_90_0/libs/asio/doc/requirements/NullaryToken.qbk
/home/garik/boost_1_90_0/libs/asio/doc/requirements/RangeConnectToken.qbk
/home/garik/boost_1_90_0/libs/asio/doc/requirements/AcceptToken.qbk
/home/garik/boost_1_90_0/libs/asio/doc/requirements/ReadToken.qbk
/home/garik/boost_1_90_0/libs/asio/doc/requirements/ShutdownToken.qbk
/home/garik/boost_1_90_0/libs/asio/doc/requirements/BufferedHandshakeToken.qbk
/home/garik/boost_1_90_0/libs/asio/doc/requirements/CancellationHandler.qbk
/home/garik/boost_1_90_0/libs/asio/doc/requirements/WriteToken.qbk
/home/garik/boost_1_90_0/libs/asio/doc/requirements/ConstBufferSequence.qbk
/home/garik/boost_1_90_0/libs/asio/doc/requirements/IteratorConnectToken.qbk
/home/garik/boost_1_90_0/libs/asio/doc/requirements/ConnectToken.qbk
/home/garik/boost_1_90_0/libs/asio/doc/requirements/Executor.qbk
/home/garik/boost_1_90_0/libs/asio/doc/reference.qbk
/home/garik/boost_1_90_0/libs/asio/doc/using.qbk
/home/garik/boost_1_90_0/libs/asio/doc/reference.xsl
/home/garik/boost_1_90_0/libs/asio/doc/std_executors.qbk
/home/garik/boost_1_90_0/libs/asio/doc/history.qbk
/home/garik/boost_1_90_0/libs/asio/doc/tutorial.qbk
/home/garik/boost_1_90_0/libs/asio/doc/examples.qbk
/home/garik/boost_1_90_0/libs/phoenix/example/adapted_echo_server.cpp
/home/garik/boost_1_90_0/libs/thread/test/test_9303.cpp
/home/garik/boost_1_90_0/libs/unordered/test/unordered/mmap_tests.cpp
/home/garik/boost_1_90_0/libs/unordered/test/cfoa/interprocess_concurrency_tests.cpp
/home/garik/boost_1_90_0/libs/cobalt/example/thread.cpp
/home/garik/boost_1_90_0/libs/cobalt/example/thread_pool.cpp
/home/garik/boost_1_90_0/libs/cobalt/example/spsc.cpp
/home/garik/boost_1_90_0/libs/cobalt/example/ticker.cpp
/home/garik/boost_1_90_0/libs/cobalt/example/http.cpp
/home/garik/boost_1_90_0/libs/cobalt/example/echo_server.cpp
/home/garik/boost_1_90_0/libs/cobalt/src/io/socket.cpp
/home/garik/boost_1_90_0/libs/cobalt/src/io/file.cpp
/home/garik/boost_1_90_0/libs/cobalt/src/io/random_access_file.cpp
/home/garik/boost_1_90_0/libs/cobalt/src/detail/exception.cpp
/home/garik/boost_1_90_0/libs/cobalt/test/with.cpp
/home/garik/boost_1_90_0/libs/cobalt/test/test.hpp
/home/garik/boost_1_90_0/libs/cobalt/test/cmake_subdir_test/main.cpp
/home/garik/boost_1_90_0/libs/cobalt/test/channel.cpp
/home/garik/boost_1_90_0/libs/cobalt/test/composition.cpp
/home/garik/boost_1_90_0/libs/cobalt/test/io/buffer.cpp
/home/garik/boost_1_90_0/libs/cobalt/test/io/endpoint.cpp
/home/garik/boost_1_90_0/libs/cobalt/test/thread.cpp
/home/garik/boost_1_90_0/libs/cobalt/test/handler.cpp
/home/garik/boost_1_90_0/libs/cobalt/test/cmake_install_test/main.cpp
/home/garik/boost_1_90_0/libs/cobalt/test/experimental/context.cpp
/home/garik/boost_1_90_0/libs/cobalt/test/experimental/yield_context.cpp
/home/garik/boost_1_90_0/libs/cobalt/test/any_completion_handler.cpp
/home/garik/boost_1_90_0/libs/cobalt/test/main.cpp
/home/garik/boost_1_90_0/libs/cobalt/test/wrappers.cpp
/home/garik/boost_1_90_0/libs/cobalt/bench/parallel.cpp
/home/garik/boost_1_90_0/libs/cobalt/doc/reference/config.adoc
/home/garik/boost_1_90_0/libs/cobalt/doc/reference/io/endpoint.adoc
/home/garik/boost_1_90_0/libs/cobalt/doc/html/index.html
/home/garik/boost_1_90_0/libs/cobalt/doc/benchmarks.adoc
/home/garik/boost_1_90_0/libs/log/src/syslog_backend.cpp
/home/garik/boost_1_90_0/libs/log/doc/tmp/sinks_reference.xml
/home/garik/boost_1_90_0/libs/mysql/example/3_advanced/http_server_cpp20/handle_request.hpp
/home/garik/boost_1_90_0/libs/mysql/example/3_advanced/http_server_cpp20/server.hpp
/home/garik/boost_1_90_0/libs/mysql/example/3_advanced/http_server_cpp20/repository.hpp
/home/garik/boost_1_90_0/libs/mysql/example/3_advanced/http_server_cpp20/handle_request.cpp
/home/garik/boost_1_90_0/libs/mysql/example/3_advanced/http_server_cpp20/repository.cpp
/home/garik/boost_1_90_0/libs/mysql/example/3_advanced/http_server_cpp20/main.cpp
/home/garik/boost_1_90_0/libs/mysql/example/3_advanced/http_server_cpp20/server.cpp
/home/garik/boost_1_90_0/libs/mysql/example/3_advanced/http_server_cpp14_coroutines/handle_request.hpp
/home/garik/boost_1_90_0/libs/mysql/example/3_advanced/http_server_cpp14_coroutines/server.hpp
/home/garik/boost_1_90_0/libs/mysql/example/3_advanced/http_server_cpp14_coroutines/repository.hpp
/home/garik/boost_1_90_0/libs/mysql/example/3_advanced/http_server_cpp14_coroutines/handle_request.cpp
/home/garik/boost_1_90_0/libs/mysql/example/3_advanced/http_server_cpp14_coroutines/repository.cpp
/home/garik/boost_1_90_0/libs/mysql/example/3_advanced/http_server_cpp14_coroutines/main.cpp
/home/garik/boost_1_90_0/libs/mysql/example/3_advanced/http_server_cpp14_coroutines/server.cpp
/home/garik/boost_1_90_0/libs/mysql/example/2_simple/unix_socket.cpp
/home/garik/boost_1_90_0/libs/mysql/example/2_simple/batch_inserts.cpp
/home/garik/boost_1_90_0/libs/mysql/example/2_simple/disable_tls.cpp
/home/garik/boost_1_90_0/libs/mysql/example/2_simple/metadata.cpp
/home/garik/boost_1_90_0/libs/mysql/example/2_simple/patch_updates.cpp
/home/garik/boost_1_90_0/libs/mysql/example/2_simple/inserts.cpp
/home/garik/boost_1_90_0/libs/mysql/example/2_simple/coroutines_cpp11.cpp
/home/garik/boost_1_90_0/libs/mysql/example/2_simple/deletes.cpp
/home/garik/boost_1_90_0/libs/mysql/example/2_simple/batch_inserts_generic.cpp
/home/garik/boost_1_90_0/libs/mysql/example/2_simple/prepared_statements.cpp
/home/garik/boost_1_90_0/libs/mysql/example/2_simple/callbacks.cpp
/home/garik/boost_1_90_0/libs/mysql/example/2_simple/pipeline.cpp
/home/garik/boost_1_90_0/libs/mysql/example/2_simple/dynamic_filters.cpp
/home/garik/boost_1_90_0/libs/mysql/example/2_simple/source_script.cpp
/home/garik/boost_1_90_0/libs/mysql/example/2_simple/multi_function.cpp
/home/garik/boost_1_90_0/libs/mysql/example/2_simple/tls_certificate_verification.cpp
/home/garik/boost_1_90_0/libs/mysql/example/1_tutorial/7_error_handling.cpp
/home/garik/boost_1_90_0/libs/mysql/example/1_tutorial/5_updates_transactions.cpp
/home/garik/boost_1_90_0/libs/mysql/example/1_tutorial/2_async.cpp
/home/garik/boost_1_90_0/libs/mysql/example/1_tutorial/3_with_params.cpp
/home/garik/boost_1_90_0/libs/mysql/example/1_tutorial/1_sync.cpp
/home/garik/boost_1_90_0/libs/mysql/example/1_tutorial/4_static_interface.cpp
/home/garik/boost_1_90_0/libs/mysql/example/1_tutorial/6_connection_pool.cpp
/home/garik/boost_1_90_0/libs/mysql/test/common/src/utils.cpp
/home/garik/boost_1_90_0/libs/mysql/test/unit/src/utils.cpp
/home/garik/boost_1_90_0/libs/mysql/test/unit/test/any_connection.cpp
/home/garik/boost_1_90_0/libs/mysql/test/unit/test/connection_pool/sansio_connection_node.cpp
/home/garik/boost_1_90_0/libs/mysql/test/unit/test/connection_pool/connection_pool_impl.cpp
/home/garik/boost_1_90_0/libs/mysql/test/unit/test/pool_params.cpp
/home/garik/boost_1_90_0/libs/mysql/test/unit/test/impl/variant_stream.cpp
/home/garik/boost_1_90_0/libs/mysql/test/unit/test/impl/ssl_context_with_default.cpp
/home/garik/boost_1_90_0/libs/mysql/test/unit/test/with_diagnostics.cpp
/home/garik/boost_1_90_0/libs/mysql/test/unit/test/spotchecks/default_completion_tokens.cpp
/home/garik/boost_1_90_0/libs/mysql/test/unit/test/spotchecks/execution_requests.cpp
/home/garik/boost_1_90_0/libs/mysql/test/unit/test/spotchecks/misc.cpp
/home/garik/boost_1_90_0/libs/mysql/test/unit/test/connection_pool.cpp
/home/garik/boost_1_90_0/libs/mysql/test/unit/test/sansio/start_execution.cpp
/home/garik/boost_1_90_0/libs/mysql/test/unit/test/sansio/quit_connection.cpp
/home/garik/boost_1_90_0/libs/mysql/test/unit/test/sansio/handshake/handshake_csha2p_encrypt_password.cpp
/home/garik/boost_1_90_0/libs/mysql/test/unit/test/sansio/top_level_algo.cpp
/home/garik/boost_1_90_0/libs/mysql/test/unit/test/sansio/close_connection.cpp
/home/garik/boost_1_90_0/libs/mysql/test/unit/test/sansio/run_pipeline.cpp
/home/garik/boost_1_90_0/libs/mysql/test/unit/test/sansio/read_some_rows.cpp
/home/garik/boost_1_90_0/libs/mysql/test/unit/test/is_fatal_error.cpp
/home/garik/boost_1_90_0/libs/mysql/test/unit/test/detail/socket_stream.cpp
/home/garik/boost_1_90_0/libs/mysql/test/unit/test/detail/engine_impl.cpp
/home/garik/boost_1_90_0/libs/mysql/test/unit/test/detail/intermediate_handler.cpp
/home/garik/boost_1_90_0/libs/mysql/test/unit/test/connection.cpp
/home/garik/boost_1_90_0/libs/mysql/test/thread_safety/connection_pool_two_contexts.cpp
/home/garik/boost_1_90_0/libs/mysql/test/thread_safety/connection_pool_cancel_get_connection.cpp
/home/garik/boost_1_90_0/libs/mysql/test/thread_safety/connection_pool_external_strand.cpp
/home/garik/boost_1_90_0/libs/mysql/test/thread_safety/connection_pool.cpp
/home/garik/boost_1_90_0/libs/mysql/test/thread_safety/connection_pool_cancel.cpp
/home/garik/boost_1_90_0/libs/mysql/test/thread_safety/connection_pool_coroutines.cpp
/home/garik/boost_1_90_0/libs/mysql/test/cmake_test/main.cpp
/home/garik/boost_1_90_0/libs/mysql/test/cmake_b2_test/main.cpp
/home/garik/boost_1_90_0/libs/mysql/test/cmake_b2_separate_compilation_test/main.cpp
/home/garik/boost_1_90_0/libs/mysql/test/fuzzing/fuzz_format_sql_injection.cpp
/home/garik/boost_1_90_0/libs/mysql/test/integration/src/utils.cpp
/home/garik/boost_1_90_0/libs/mysql/test/integration/test/character_set_tracking.cpp
/home/garik/boost_1_90_0/libs/mysql/test/integration/test/any_connection.cpp
/home/garik/boost_1_90_0/libs/mysql/test/integration/test/snippets/dynamic_interface.cpp
/home/garik/boost_1_90_0/libs/mysql/test/integration/test/snippets/tutorials.cpp
/home/garik/boost_1_90_0/libs/mysql/test/integration/test/snippets/templated_connection.cpp
/home/garik/boost_1_90_0/libs/mysql/test/integration/test/snippets/sql_formatting_advanced.cpp
/home/garik/boost_1_90_0/libs/mysql/test/integration/test/snippets/overview.cpp
/home/garik/boost_1_90_0/libs/mysql/test/integration/test/snippets/connection_establishment.cpp
/home/garik/boost_1_90_0/libs/mysql/test/integration/test/snippets/interfacing_sync_async.cpp
/home/garik/boost_1_90_0/libs/mysql/test/integration/test/snippets/connection_pool.cpp
/home/garik/boost_1_90_0/libs/mysql/test/integration/test/snippets/prepared_statements.cpp
/home/garik/boost_1_90_0/libs/mysql/test/integration/test/snippets/static_interface.cpp
/home/garik/boost_1_90_0/libs/mysql/test/integration/test/snippets/multi_resultset.cpp
/home/garik/boost_1_90_0/libs/mysql/test/integration/test/snippets/text_queries.cpp
/home/garik/boost_1_90_0/libs/mysql/test/integration/test/spotchecks.cpp
/home/garik/boost_1_90_0/libs/mysql/test/integration/test/connection_id.cpp
/home/garik/boost_1_90_0/libs/mysql/test/integration/test/connection_pool.cpp
/home/garik/boost_1_90_0/libs/mysql/test/integration/test/reconnect.cpp
/home/garik/boost_1_90_0/libs/mysql/test/integration/test/handshake.cpp
/home/garik/boost_1_90_0/libs/mysql/test/integration/test/execution_requests.cpp
/home/garik/boost_1_90_0/libs/mysql/test/integration/test/pipeline.cpp
/home/garik/boost_1_90_0/libs/mysql/test/integration/include/test_integration/run_coro.hpp
/home/garik/boost_1_90_0/libs/mysql/test/integration/include/test_integration/snippets/get_connection.hpp
/home/garik/boost_1_90_0/libs/mysql/bench/many_rows_boost.cpp
/home/garik/boost_1_90_0/libs/mysql/bench/connection_pool.cpp
/home/garik/boost_1_90_0/libs/mysql/bench/one_small_row_boost.cpp
/home/garik/boost_1_90_0/libs/mysql/bench/one_big_row_boost.cpp
/home/garik/boost_1_90_0/libs/mysql/bench/stmt_params_boost.cpp
/home/garik/boost_1_90_0/libs/mysql/doc/qbk/19_templated_connection.qbk
/home/garik/boost_1_90_0/libs/mysql/doc/qbk/helpers/Stream.qbk
/home/garik/boost_1_90_0/libs/mysql/doc/qbk/helpers/SocketStream.qbk
/home/garik/boost_1_90_0/libs/mysql/doc/qbk/03_2_tutorial_async.qbk
/home/garik/boost_1_90_0/libs/coroutine/doc/html/coroutine/motivation.html
/home/garik/boost_1_90_0/libs/coroutine/doc/motivation.qbk
/home/garik/boost_1_90_0/libs/coroutine/doc/coro.qbk
/home/garik/boost_1_90_0/libs/url/example/router/router.cpp
/home/garik/boost_1_90_0/libs/url/doc/modules/ROOT/examples/example/router.cpp
/home/garik/boost_1_90_0/libs/fiber/examples/asio/autoecho.cpp
/home/garik/boost_1_90_0/libs/fiber/examples/asio/ps/publisher.cpp
/home/garik/boost_1_90_0/libs/fiber/examples/asio/ps/subscriber.cpp
/home/garik/boost_1_90_0/libs/fiber/examples/asio/ps/server.cpp
/home/garik/boost_1_90_0/libs/fiber/examples/asio/round_robin.hpp
/home/garik/boost_1_90_0/libs/fiber/examples/asio/exchange.cpp
/home/garik/boost_1_90_0/libs/fiber/doc/integration.qbk
/home/garik/boost_1_90_0/libs/fiber/doc/fibers.qbk
/home/garik/boost_1_90_0/libs/fiber/doc/callbacks.qbk
/home/garik/boost_1_90_0/libs/fiber/doc/asio.qbk
/home/garik/boost_1_90_0/libs/process/example/stdio.cpp
/home/garik/boost_1_90_0/libs/process/example/intro.cpp
/home/garik/boost_1_90_0/libs/process/example/intro_popen.cpp
/home/garik/boost_1_90_0/libs/process/example/quickstart.cpp
/home/garik/boost_1_90_0/libs/process/example/env.cpp
/home/garik/boost_1_90_0/libs/process/example/start_dir.cpp
/home/garik/boost_1_90_0/libs/process/test/v1/system_test1.cpp
/home/garik/boost_1_90_0/libs/process/test/v1/async_pipe.cpp
/home/garik/boost_1_90_0/libs/process/test/v1/wait.cpp
/home/garik/boost_1_90_0/libs/process/test/v1/spawn_fail.cpp
/home/garik/boost_1_90_0/libs/process/test/v1/async_fut.cpp
/home/garik/boost_1_90_0/libs/process/test/v1/exit_code.cpp
/home/garik/boost_1_90_0/libs/process/test/v1/bind_stdin.cpp
/home/garik/boost_1_90_0/libs/process/test/v1/async_system_stackful.cpp
/home/garik/boost_1_90_0/libs/process/test/v1/async_system_stackful_except.cpp
/home/garik/boost_1_90_0/libs/process/test/v1/limit_fd.cpp
/home/garik/boost_1_90_0/libs/process/test/v1/on_exit2.cpp
/home/garik/boost_1_90_0/libs/process/test/v1/bind_stderr.cpp
/home/garik/boost_1_90_0/libs/process/test/v1/bind_stdout_stderr.cpp
/home/garik/boost_1_90_0/libs/process/test/v1/bind_stdout.cpp
/home/garik/boost_1_90_0/libs/process/test/v1/async_system_stackful_error.cpp
/home/garik/boost_1_90_0/libs/process/test/v1/async_system_stackless.cpp
/home/garik/boost_1_90_0/libs/process/test/v1/system_test2.cpp
/home/garik/boost_1_90_0/libs/process/test/v1/async_system_future.cpp
/home/garik/boost_1_90_0/libs/process/test/v1/spawn.cpp
/home/garik/boost_1_90_0/libs/process/test/v1/async_system_fail.cpp
/home/garik/boost_1_90_0/libs/process/test/v1/on_exit.cpp
/home/garik/boost_1_90_0/libs/process/test/v1/on_exit3.cpp
/home/garik/boost_1_90_0/libs/process/test/v1/posix_specific.cpp
/home/garik/boost_1_90_0/libs/process/test/v1/async.cpp
/home/garik/boost_1_90_0/libs/process/test/v2/process.cpp
/home/garik/boost_1_90_0/libs/process/test/v2/pid.cpp
/home/garik/boost_1_90_0/libs/process/test/v2/target.cpp
/home/garik/boost_1_90_0/libs/process/test/v2/windows.cpp
/home/garik/boost_1_90_0/libs/process/test/v2/shell.cpp
/home/garik/boost_1_90_0/libs/process/test/v2/ext.cpp
/home/garik/boost_1_90_0/libs/mqtt5/example/timeout_with_parallel_group.cpp
/home/garik/boost_1_90_0/libs/mqtt5/example/hello_world_over_tls.cpp
/home/garik/boost_1_90_0/libs/mqtt5/example/publisher.cpp
/home/garik/boost_1_90_0/libs/mqtt5/example/hello_world_in_multithreaded_env.cpp
/home/garik/boost_1_90_0/libs/mqtt5/example/hello_world_in_coro_multithreaded_env.cpp
/home/garik/boost_1_90_0/libs/mqtt5/example/timeout_with_awaitable_operators.cpp
/home/garik/boost_1_90_0/libs/mqtt5/example/multiflight_client.cpp
/home/garik/boost_1_90_0/libs/mqtt5/example/hello_world_over_websocket_tcp.cpp
/home/garik/boost_1_90_0/libs/mqtt5/example/hello_world_over_websocket_tls.cpp
/home/garik/boost_1_90_0/libs/mqtt5/example/receiver.cpp
/home/garik/boost_1_90_0/libs/mqtt5/example/hello_world_over_tcp.cpp
/home/garik/boost_1_90_0/libs/mqtt5/test/src/quick.cpp
/home/garik/boost_1_90_0/libs/mqtt5/test/unit/logger.cpp
/home/garik/boost_1_90_0/libs/mqtt5/test/unit/traits.cpp
/home/garik/boost_1_90_0/libs/mqtt5/test/include/test_common/test_stream.hpp
/home/garik/boost_1_90_0/libs/mqtt5/test/include/test_common/test_authenticators.hpp
/home/garik/boost_1_90_0/libs/mqtt5/test/include/test_common/delayed_op.hpp
/home/garik/boost_1_90_0/libs/mqtt5/test/include/test_common/test_broker.hpp
/home/garik/boost_1_90_0/libs/mqtt5/test/include/test_common/test_service.hpp
/home/garik/boost_1_90_0/libs/mqtt5/test/include/test_common/packet_util.hpp
/home/garik/boost_1_90_0/libs/mqtt5/test/include/test_common/test_autoconnect_stream.hpp
/home/garik/boost_1_90_0/libs/mqtt5/test/integration/client.cpp
/home/garik/boost_1_90_0/libs/mqtt5/test/integration/mqtt_features.cpp
/home/garik/boost_1_90_0/libs/mqtt5/README.md
/home/garik/boost_1_90_0/libs/mqtt5/doc/html/mqtt5/intro.html
/home/garik/boost_1_90_0/libs/mqtt5/doc/html/mqtt5/receiver.html
/home/garik/boost_1_90_0/libs/mqtt5/doc/html/mqtt5/ref/Authenticator.html
/home/garik/boost_1_90_0/libs/mqtt5/doc/html/mqtt5/ref/StreamType.html
/home/garik/boost_1_90_0/libs/mqtt5/doc/html/mqtt5/ref/boost__mqtt5__mqtt_client/async_unsubscribe/overload1.html
/home/garik/boost_1_90_0/libs/mqtt5/doc/html/mqtt5/ref/boost__mqtt5__mqtt_client/async_unsubscribe/overload2.html
/home/garik/boost_1_90_0/libs/mqtt5/doc/html/mqtt5/ref/boost__mqtt5__mqtt_client/async_receive.html
/home/garik/boost_1_90_0/libs/mqtt5/doc/html/mqtt5/ref/boost__mqtt5__mqtt_client/async_subscribe/overload1.html
/home/garik/boost_1_90_0/libs/mqtt5/doc/html/mqtt5/ref/boost__mqtt5__mqtt_client/async_subscribe/overload2.html
/home/garik/boost_1_90_0/libs/mqtt5/doc/html/mqtt5/ref/boost__mqtt5__mqtt_client/async_publish.html
/home/garik/boost_1_90_0/libs/mqtt5/doc/html/mqtt5/ref/boost__mqtt5__mqtt_client/async_disconnect/overload1.html
/home/garik/boost_1_90_0/libs/mqtt5/doc/html/mqtt5/ref/boost__mqtt5__mqtt_client/async_disconnect/overload2.html
/home/garik/boost_1_90_0/libs/mqtt5/doc/html/mqtt5/ref/boost__mqtt5__mqtt_client/async_run.html
/home/garik/boost_1_90_0/libs/mqtt5/doc/html/mqtt5/ref/TlsContext.html
/home/garik/boost_1_90_0/libs/mqtt5/doc/html/mqtt5/hello_world_over_websocket_tls.html
/home/garik/boost_1_90_0/libs/mqtt5/doc/html/mqtt5/hello_world_in_coro_multithreaded_env.html
/home/garik/boost_1_90_0/libs/mqtt5/doc/html/mqtt5/publisher.html
/home/garik/boost_1_90_0/libs/mqtt5/doc/html/mqtt5/hello_world_over_websocket_tcp.html
/home/garik/boost_1_90_0/libs/mqtt5/doc/html/mqtt5/timeout_with_awaitable_operators.html
/home/garik/boost_1_90_0/libs/mqtt5/doc/html/mqtt5/multiflight_client.html
/home/garik/boost_1_90_0/libs/mqtt5/doc/html/mqtt5/optimising_communication.html
/home/garik/boost_1_90_0/libs/mqtt5/doc/html/mqtt5/timeout_with_parallel_group.html
/home/garik/boost_1_90_0/libs/mqtt5/doc/html/mqtt5/hello_world_over_tcp.html
/home/garik/boost_1_90_0/libs/mqtt5/doc/html/mqtt5/hello_world_over_tls.html
/home/garik/boost_1_90_0/libs/mqtt5/doc/html/mqtt5/getting_started.html
/home/garik/boost_1_90_0/libs/mqtt5/doc/qbk/reference/Error_handling.qbk
/home/garik/boost_1_90_0/libs/mqtt5/doc/qbk/09_per_op_cancellation.qbk
/home/garik/boost_1_90_0/libs/mqtt5/doc/qbk/01_intro.qbk
/home/garik/boost_1_90_0/libs/mqtt5/doc/qbk/06_disconnecting_the_client.qbk
/home/garik/boost_1_90_0/libs/mqtt5/doc/qbk/11_multithreading.qbk
/home/garik/boost_1_90_0/libs/mqtt5/doc/qbk/00_main.qbk
/home/garik/boost_1_90_0/libs/mqtt5/doc/qbk/08_allocators.qbk
/home/garik/boost_1_90_0/libs/mqtt5/doc/qbk/10_executors.qbk
/home/garik/boost_1_90_0/libs/mqtt5/doc/qbk/02_getting_started.qbk
/home/garik/boost_1_90_0/tools/cmake/test/mysql/main.cpp
/home/garik/boost_1_90_0/tools/docca/include/docca/base-config.xsl
/home/garik/boost_1_90_0/doc/html/boost_asio/overview/core/strands.html
/home/garik/boost_1_90_0/doc/html/boost_asio/overview/core/allocation.html
/home/garik/boost_1_90_0/doc/html/boost_asio/overview/core/cancellation.html
/home/garik/boost_1_90_0/doc/html/boost_asio/overview/core/line_based.html
/home/garik/boost_1_90_0/doc/html/boost_asio/overview/core/buffers.html
/home/garik/boost_1_90_0/doc/html/boost_asio/overview/composition/deferred.html
/home/garik/boost_1_90_0/doc/html/boost_asio/overview/composition/coro.html
/home/garik/boost_1_90_0/doc/html/boost_asio/reference/yield_context.html
/home/garik/boost_1_90_0/doc/html/boost_asio/reference/is_error_code_enum_lt__basic_errors__gt_/value.html
/home/garik/boost_1_90_0/doc/html/boost_asio/reference/is_error_code_enum_lt__ssl_errors__gt_/value.html
/home/garik/boost_1_90_0/doc/html/boost_asio/reference/execution_context/make_service.html
/home/garik/boost_1_90_0/doc/html/boost_asio/reference/execution_context/add_service.html
/home/garik/boost_1_90_0/doc/html/boost_asio/reference/is_error_code_enum_lt__addrinfo_errors__gt_/value.html
/home/garik/boost_1_90_0/doc/html/boost_asio/reference/is_error_code_enum_lt__addrinfo_errors__gt_.html
/home/garik/boost_1_90_0/doc/html/boost_asio/reference/async_connect/overload1.html
/home/garik/boost_1_90_0/doc/html/boost_asio/reference/async_connect/overload2.html
/home/garik/boost_1_90_0/doc/html/boost_asio/reference/async_connect/overload3.html
/home/garik/boost_1_90_0/doc/html/boost_asio/reference/async_connect/overload4.html
/home/garik/boost_1_90_0/doc/html/boost_asio/reference/is_error_code_enum_lt__netdb_errors__gt_.html
/home/garik/boost_1_90_0/doc/html/boost_asio/reference/is_error_code_enum_lt__boost__asio__ssl__error__stream_errors__gt_/value.html
/home/garik/boost_1_90_0/doc/html/boost_asio/reference/experimental__coro.html
/home/garik/boost_1_90_0/doc/html/boost_asio/reference/is_error_code_enum_lt__misc_errors__gt_.html
/home/garik/boost_1_90_0/doc/html/boost_asio/reference/associated_immediate_executor_t.html
/home/garik/boost_1_90_0/doc/html/boost_asio/reference/is_error_code_enum_lt__misc_errors__gt_/value.html
/home/garik/boost_1_90_0/doc/html/boost_asio/reference/associated_immediate_executor_lt__reference_wrapper_lt__T__gt__comma__Executor__gt_/type.html
/home/garik/boost_1_90_0/doc/html/boost_asio/reference/placeholders__results.html
/home/garik/boost_1_90_0/doc/html/boost_asio/reference/default_completion_token_t.html
/home/garik/boost_1_90_0/doc/html/boost_asio/reference/is_error_code_enum_lt__ssl_errors__gt_.html
/home/garik/boost_1_90_0/doc/html/boost_asio/reference/io_context.html
/home/garik/boost_1_90_0/doc/html/boost_asio/reference/io_context__strand.html
/home/garik/boost_1_90_0/doc/html/boost_asio/reference/default_completion_token.html
/home/garik/boost_1_90_0/doc/html/boost_asio/reference/is_error_code_enum_lt__boost__asio__ssl__error__stream_errors__gt_.html
/home/garik/boost_1_90_0/doc/html/boost_asio/reference/is_error_code_enum_lt__boost__asio__experimental__error__channel_errors__gt_.html
/home/garik/boost_1_90_0/doc/html/boost_asio/reference/associated_immediate_executor.html
/home/garik/boost_1_90_0/doc/html/boost_asio/reference/is_error_code_enum_lt__boost__asio__experimental__error__channel_errors__gt_/value.html
/home/garik/boost_1_90_0/doc/html/boost_asio/reference/is_error_code_enum_lt__netdb_errors__gt_/value.html
/home/garik/boost_1_90_0/doc/html/boost_asio/reference/experimental__use_coro.html
/home/garik/boost_1_90_0/doc/html/boost_asio/reference/is_error_code_enum_lt__basic_errors__gt_.html
/home/garik/boost_1_90_0/doc/html/boost_asio/reference/experimental__task.html
/home/garik/boost_1_90_0/doc/html/boost_asio/reference/experimental__generator.html
/home/garik/boost_1_90_0/doc/html/boost_asio/reference/ip__address__gt_.html
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp20/coroutines/echo_server_with_as_single_default.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp20/coroutines/echo_server_with_as_tuple_default.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp20/coroutines/refactored_echo_server.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp20/coroutines/echo_server_with_deferred.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp20/coroutines/echo_server_with_deferred_default.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp20/coroutines/echo_server_with_default.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp20/coroutines/chat_server.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp20/coroutines/timeout.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp20/coroutines/echo_server.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp20/channels/throttling_proxy.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp20/channels/mutual_exclusion_1.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp20/channels/mutual_exclusion_2.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp20/invocation/completion_executor.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp20/operations/composed_3.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp20/operations/composed_6.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp20/operations/composed_4.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp20/operations/composed_2.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp20/operations/callback_wrapper.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp20/operations/c_callback_wrapper.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp20/operations/composed_5.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp20/operations/composed_1.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp20/operations/composed_8.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp20/operations/composed_7.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp20/type_erasure/sleep.hpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp20/type_erasure/stdin_line_reader.hpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp20/type_erasure/stdin_line_reader.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp20/type_erasure/sleep.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp20/type_erasure/line_reader.hpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp20/type_erasure/main.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp11/multicast/sender.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp11/multicast/receiver.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp11/ssl/client.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp11/ssl/server.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp11/buffers/reference_counted.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp11/timers/time_t_timer.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp11/handler_tracking/custom_tracking.hpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp11/handler_tracking/async_tcp_echo_server.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp11/allocation/server.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp11/spawn/echo_server.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp11/spawn/parallel_grep.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp11/http/server3/reply.hpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp11/http/server3/server.hpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp11/http/server3/reply.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp11/http/server3/connection.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp11/http/server3/server.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp11/http/server3/connection.hpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp11/http/client/async_client.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp11/http/client/sync_client.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp11/http/server2/io_context_pool.hpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp11/http/server2/reply.hpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp11/http/server2/server.hpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp11/http/server2/reply.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp11/http/server2/io_context_pool.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp11/http/server2/connection.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp11/http/server2/server.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp11/http/server2/connection.hpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp11/http/server4/reply.hpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp11/http/server4/server.hpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp11/http/server4/reply.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp11/http/server4/main.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp11/http/server4/server.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp11/http/server/reply.hpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp11/http/server/server.hpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp11/http/server/reply.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp11/http/server/connection.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp11/http/server/server.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp11/http/server/connection.hpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp11/serialization/client.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp11/serialization/server.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp11/serialization/connection.hpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp11/windows/transmit_file.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp11/iostreams/daytime_client.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp11/iostreams/http_client.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp11/iostreams/daytime_server.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp11/socks4/socks4.hpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp11/socks4/sync_client.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp11/chat/chat_client.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp11/chat/posix_chat_client.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp11/chat/chat_server.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp11/local/iostream_client.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp11/local/fd_passing_stream_server.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp11/local/fd_passing_stream_client.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp11/local/stream_client.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp11/local/stream_server.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp11/local/connect_pair.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp11/timeouts/blocking_tcp_client.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp11/timeouts/blocking_udp_client.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp11/timeouts/blocking_token_tcp_client.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp11/timeouts/async_tcp_client.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp11/timeouts/server.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp11/icmp/ping.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp11/icmp/ipv4_header.hpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp11/futures/daytime_client.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp11/nonblocking/third_party_lib.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp11/deferred/deferred_2.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp11/deferred/deferred_1.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp11/invocation/prioritised_handlers.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp11/fork/process_per_connection.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp11/fork/daemon.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp11/operations/composed_3.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp11/operations/composed_6.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp11/operations/composed_4.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp11/operations/composed_2.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp11/operations/composed_5.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp11/operations/composed_1.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp11/operations/composed_8.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp11/operations/composed_7.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp11/parallel_group/wait_for_all.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp11/parallel_group/wait_for_one.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp11/parallel_group/wait_for_one_success.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp11/parallel_group/wait_for_one_error.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp11/parallel_group/ranged_wait_for_all.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp11/executors/bank_account_2.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp11/executors/bank_account_1.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp11/executors/actor.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp11/executors/fork_join.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp11/executors/priority_scheduler.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp11/executors/pipeline.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp11/type_erasure/sleep.hpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp11/type_erasure/stdin_line_reader.hpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp11/type_erasure/stdin_line_reader.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp11/type_erasure/sleep.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp11/type_erasure/line_reader.hpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp11/type_erasure/main.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp11/porthopper/client.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp11/porthopper/protocol.hpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp11/porthopper/server.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp11/services/daytime_client.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp11/services/basic_logger.hpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp11/services/logger_service.hpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp11/echo/blocking_tcp_echo_server.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp11/echo/blocking_udp_echo_server.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp11/echo/blocking_udp_echo_client.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp11/echo/async_udp_echo_server.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp11/echo/async_tcp_echo_server.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp11/echo/blocking_tcp_echo_client.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp17/coroutines_ts/echo_server_with_as_single_default.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp17/coroutines_ts/echo_server_with_as_tuple_default.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp17/coroutines_ts/refactored_echo_server.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp17/coroutines_ts/echo_server_with_default.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp17/coroutines_ts/range_based_for.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp17/coroutines_ts/chat_server.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp17/coroutines_ts/echo_server.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp14/iostreams/http_client.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp14/deferred/deferred_2.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp14/deferred/deferred_7.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp14/deferred/deferred_5.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp14/deferred/deferred_4.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp14/deferred/deferred_6.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp14/deferred/deferred_3.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp14/deferred/deferred_1.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp14/operations/composed_3.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp14/operations/composed_6.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp14/operations/composed_4.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp14/operations/composed_2.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp14/operations/callback_wrapper.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp14/operations/c_callback_wrapper.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp14/operations/composed_5.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp14/operations/composed_1.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp14/operations/composed_8.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp14/operations/composed_7.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp14/parallel_group/wait_for_all.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp14/parallel_group/wait_for_one.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp14/parallel_group/wait_for_one_success.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp14/parallel_group/wait_for_one_error.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp14/parallel_group/parallel_sort.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp14/parallel_group/ranged_wait_for_all.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp14/executors/bank_account_2.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp14/executors/bank_account_1.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp14/executors/async_1.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp14/executors/actor.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp14/executors/async_2.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp14/executors/fork_join.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp14/executors/priority_scheduler.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp14/executors/pipeline.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp14/echo/blocking_tcp_echo_server.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp14/echo/blocking_udp_echo_server.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp14/echo/blocking_udp_echo_client.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp14/echo/async_udp_echo_server.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp14/echo/async_tcp_echo_server.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/example/cpp14/echo/blocking_tcp_echo_client.cpp
/home/garik/boost_1_90_0/doc/html/boost_asio/examples/cpp11_examples.html
/home/garik/boost_1_90_0/doc/html/boost_asio/std_executors.html
/home/garik/boost_1_90_0/doc/html/boost_asio/index.html
/home/garik/boost_1_90_0/doc/html/boost_asio/tutorial/tuttimer2.html
/home/garik/boost_1_90_0/doc/html/boost_asio/tutorial/tuttimer1.html
/home/garik/boost_1_90_0/doc/html/boost_asio/tutorial/tuttimer4.html
/home/garik/boost_1_90_0/doc/html/boost_asio/tutorial/tutdaytime3.html
/home/garik/boost_1_90_0/doc/html/boost_asio/tutorial/tutdaytime1.html
/home/garik/boost_1_90_0/doc/html/boost_asio/tutorial/tutdaytime6.html
/home/garik/boost_1_90_0/doc/html/boost_asio/tutorial/tuttimer5.html
/home/garik/boost_1_90_0/doc/html/boost_asio/tutorial/tuttimer3.html
/home/garik/boost_1_90_0/doc/antora/url/examples/router.html
/home/garik/boost_1_90_0/stage/lib/libboost_log.a
/home/garik/boost_1_90_0/stage/lib/libboost_log.so.1.90.0

8.Скомпилируйте boost
Решение: cd  ~/boost_1_90_0
         ./bootstrap.sh
Вывод :Building B2 engine..

###
###
### Using 'gcc' toolset.
###
###

g++ (Debian 14.2.0-19) 14.2.0
Copyright (C) 2024 Free Software Foundation, Inc.
This is free software; see the source for copying conditions.  There is NO
warranty; not even for MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.


###
###

> g++ -x c++ -std=c++11 -pthread -O2 -s -DNDEBUG bindjam.cpp builtins.cpp class.cpp command.cpp compile.cpp constants.cpp cwd.cpp debug.cpp debugger.cpp events.cpp execcmd.cpp execnt.cpp execunix.cpp filent.cpp filesys.cpp fileunix.cpp frames.cpp function.cpp glob.cpp hash.cpp hcache.cpp hdrmacro.cpp headers.cpp jam_strings.cpp jam.cpp jamgram.cpp lists.cpp make.cpp make1.cpp md5.cpp mem.cpp modules.cpp native.cpp output.cpp parse.cpp pathnt.cpp pathsys.cpp pathunix.cpp regexp.cpp rules.cpp scan.cpp search.cpp startup.cpp tasks.cpp timestamp.cpp value.cpp variable.cpp w32_getreg.cpp mod_args.cpp mod_command_db.cpp mod_db.cpp mod_jam_builtin.cpp mod_jam_class.cpp mod_jam_errors.cpp mod_jam_modules.cpp mod_order.cpp mod_path.cpp mod_property_set.cpp mod_regex.cpp mod_sequence.cpp mod_set.cpp mod_string.cpp mod_summary.cpp mod_sysinfo.cpp mod_version.cpp -o b2
tools/build/src/engine/b2
Unicode/ICU support for Boost.Regex?... not found.
Backing up existing B2 configuration in project-config.jam.1
Generating B2 configuration in project-config.jam for gcc...

Bootstrapping is done. To build, run:

    ./b2
    
To generate header files, run:

    ./b2 headers

The configuration generated uses gcc to build by default. If that is
unintended either use the --with-toolset option or adjust configuration, by
editing 'project-config.jam'.

Further information:

   - Command line help:
     ./b2 --help
     
   - Getting started guide: 
     http://www.boost.org/more/getting_started/unix-variants.html
     
   - B2 documentation:
     http://www.boost.org/build/
   
 
Далее: ./b2 --build-dir=/tmp/build-boost toolset=gcc stage
Вывод: ...updated 2220 targets...


10.Подсчитайте сколько занимает дискового пространства каждый файл в этой директории.
Решение: cd ~/boost-libs, далее: du -sh *
Вывод:
 20K	libboost_atomic.a
284K	libboost_charconv.a
148K	libboost_chrono.a
164K	libboost_container.a
12K	libboost_context.a
256K	libboost_contract.a
32K	libboost_coroutine.a
4.0K	libboost_date_time.a
4.0K	libboost_exception.a
252K	libboost_fiber.a
420K	libboost_filesystem.a
940K	libboost_graph.a
128K	libboost_iostreams.a
764K	libboost_json.a
1.7M	libboost_locale.a
2.9M	libboost_log.a
2.7M	libboost_log_setup.a
104K	libboost_math_c99.a
104K	libboost_math_c99f.a
100K	libboost_math_c99l.a
852K	libboost_math_tr1.a
912K	libboost_math_tr1f.a
844K	libboost_math_tr1l.a
20K	libboost_nowide.a
172K	libboost_prg_exec_monitor.a
484K	libboost_process.a
1.1M	libboost_program_options.a
52K	libboost_random.a
724K	libboost_regex.a
1.2M	libboost_serialization.a
48K	libboost_stacktrace_addr2line.a
40K	libboost_stacktrace_backtrace.a
32K	libboost_stacktrace_basic.a
8.0K	libboost_stacktrace_from_exception.a
4.0K	libboost_stacktrace_noop.a
2.2M	libboost_test_exec_monitor.a
284K	libboost_thread.a
24K	libboost_timer.a
116K	libboost_type_erasure.a
2.2M	libboost_unit_test_framework.a
2.3M	libboost_url.a
4.4M	libboost_wave.a
772K	libboost_wserialization.a

11.Найдите топ10 самых "тяжёлых".
Решение: cd ~/boost-libs, далее: du -sh * | sort -rh | head -10
Вывод: 
4.4M	libboost_wave.a
2.9M	libboost_log.a
2.7M	libboost_log_setup.a
2.3M	libboost_url.a
2.2M	libboost_unit_test_framework.a
2.2M	libboost_test_exec_monitor.a
1.7M	libboost_locale.a
1.2M	libboost_serialization.a
1.1M	libboost_program_options.a
940K	libboost_graph.a


# Copyright 2018, 2019 Peter Dimov
# Copyright 2023 Matt Borland
# Distributed under the Boost Software License, Version 1.0.
# See accompanying file LICENSE_1_0.txt or copy at http://www.boost.org/LICENSE_1_0.txt

include(BoostTestJamfile OPTIONAL RESULT_VARIABLE HAVE_BOOST_TEST)

if(HAVE_BOOST_TEST)

    boost_test_jamfile(FILE Jamfile LINK_LIBRARIES Boost::int128 Boost::core Boost::random Boost::multiprecision Boost::mp11 Boost::charconv)

endif()

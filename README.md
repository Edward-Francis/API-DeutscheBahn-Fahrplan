# NAME

API::DeutscheBahn::Fahrplan - Deutsche Bahn Fahrplan API Client

# SYNOPSIS

    my $fahrplan_free = API::DeutscheBahn::Fahrplan->new;
    my $fahrplan_plus = API::DeutscheBahn::Fahrplan->new( access_token => $access_token );

    $data = $fahrplan->location( name => 'Berlin' );
    $data = $fahrplan->arrival_board( id => 8503000, date => '2018-09-24T11:00:00' );
    $data = $fahrplan->departure_board( id => 8503000, date => '2018-09-24T11:00:00' );
    $data = $fahrplan->journey_details( id => '87510%2F49419%2F965692%2F453678%2F80%3fstation_evaId%3D850300' );

# DESCRIPTION

API::DeutscheBahn::Fahrplan provides a simple interface to the Deutsche Bahn Fahrplan
API. See [Deutsche Bahn API](https://developer.deutschebahn.com/) for further information.

# LICENSE

Copyright (C) Edward Francis.

This library is free software; you can redistribute it and/or modify
it under the same terms as Perl itself.

# AUTHOR

Edward Francis <edwardafrancis@gmail.com>

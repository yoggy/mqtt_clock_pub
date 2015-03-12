mqtt_clock_pub
====
publish the local time using the MQTT.

setup
----
    $ sudo gem install mqtt
    $ sudo gem install pit

how to use
----
    $ git https://github.com/yoggy/mqtt_clock_pub.git
    $ cd mqtt_clock_pub
    $ EDITOR=vim ruby mqtt_clock_pub.rb
    
        ---
        remote_host: mqtt.example.com
        remote_port: 1883
        use_auth: false
        username: username
        password: password
        topic: publish_topic

    connected!
    {"epoch":1426150733,"iso8601":"2015-03-12T17:58:53+09:00"}
    {"epoch":1426150734,"iso8601":"2015-03-12T17:58:54+09:00"}
    {"epoch":1426150735,"iso8601":"2015-03-12T17:58:55+09:00"}
    {"epoch":1426150736,"iso8601":"2015-03-12T17:58:56+09:00"}
        .
        .
        .
        .


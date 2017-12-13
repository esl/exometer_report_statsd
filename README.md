# exometer_report_statsd

#### <a name="Configuring_statsd_reporter">Configuring StatsD reporter</a> ####

Below is an example of the StatsD reporter application environment, with
its correct location in the hierarchy:

```erlang

{exometer_core, [
    {report, [
        {reporters, [
            {exometer_report_statsd, [
                {hostname, "testhost"},
                {port, 4125},
                {prefix, "prefix_"},
                {type_map, []}
            ]}
        ]}
    ]}
]}
```

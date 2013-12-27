new development on allwinner a10

performance on arm board :

echo 'governor="performance"'>>/etc/default/cpupower

echo ondemand > /sys/devices/system/cpu/cpu0/cpufreq/scaling_governor
 
echo 1008000 > /sys/devices/system/cpu/cpu0/cpufreq/scaling_max_freq
echo 408000 > /sys/devices/system/cpu/cpu0/cpufreq/scaling_min_freq
 
echo 25 > /sys/devices/system/cpu/cpufreq/ondemand/up_threshold
echo 10 > /sys/devices/system/cpu/cpufreq/ondemand/sampling_down_factor
echo 1 > /sys/devices/system/cpu/cpufreq/ondemand/io_is_busy

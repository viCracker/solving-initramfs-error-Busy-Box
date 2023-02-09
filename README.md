# solving-initramfs-error-Busy-Box
This is a repository about How to fix the Busy Box error/initramfs from the prompted command line

I encounted this Error on my Kali linux recently and This is how I solved it
This is error could come up as a result of several issues but the most common one is an error about inconsistency of a file sytem which needs to be fixed hence solving the error.Initramfs stands for initial RAM filesystem which is loaded by the kernel during the boot process.

Step1:
type exit command to find the issue.It generates a report showing the disk device for example /dev/sda1 with the inconsistency and illustrated UNEXPECTED INCONSISTENCY as the error.

Step2:
Solving the inconsistency using fsck. we use fsck which is a command used to check and repair filesystems.
type fsck /dev/sda1 -y and click enter. The command here assumes your disk is /dev/sda1, y is an option to answer yes to all prompted questions. 
This will generate a report showing successfull completion of the process.

Step3:
Type reboot on your command line to restart your computer with the solution solved.

THIS INFORMATION IS INTENDED TO GIVE YOU EDUCATION. YOU CAN THEN USE YOUR EDUCATION IN ANY WAY. EITHER WAY I SHOULD NOT BE HELD RESPONSIBLE FOR ANY ILLEGAL ACTIVITY CARRIED OUT USING THE ABOVE INFORMATION

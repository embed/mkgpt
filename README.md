mkgpt is a simple tool to create an empty GUID Partition Table on a device. It's usage is simple:

    mkgpt [--force] device

where *device* is the destination device. If the tool detects an existing partition table on it, it will refuse to proceed. If you still want to proceed (and destroy your existing partition scheme), use the --force parameter

# How to build
Simply type:

    make

and a binary called mkgpt will be produced. There is another utility called gptdump. It shows the contents of the primary and secondary GPT. To build it, type:

    make gptdump

Usage:

    gptdump device


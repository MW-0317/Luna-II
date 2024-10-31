env = Environment()

srcs = ['main/main.c']
incs = ['thirdparty/**']
localincs = []
resources = []
misc = []

dll = env.SharedLibrary(target = "lunaII.dll",
                        source = srcs)

env.MSVSProject(target = "LunaII" + env['MSVSPROJECTSUFFIX'],
                srcs = srcs,
                incs = incs,
                localincs = localincs,
                resources = resources,
                misc = misc,
                buildtarget = dll[0],
                variant = ["Release"])
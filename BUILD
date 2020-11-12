# rules_go boilerplate
load("@bazel_gazelle//:def.bzl", "gazelle")

# update_deb_packages boilerplate
load("@rules_dpkg//tools/update_deb_packages:update_deb_packages.bzl", "update_deb_packages")

package(default_visibility = ["//visibility:public"])

gazelle(
    name = "gazelle",
    prefix = "github.com/mariusgrigoriu/rules_dpkg",
)

update_deb_packages(
    name = "update_deb_packages",
    pgp_keys = [
        "@jessie_archive_key//file",
        "@stretch_archive_key//file",
    ],
)

ansible-prepare-host
====================

Take a new stack created in Sandvine's Nubo, and make it yours.
Make it so that you can use git to save/restore your config,
that your vi works the way you need, etc.

To set it up, cp params.yml.sample to params.yml, and edit
to suit.

Then run

ansible-playbook -v -u cloud -i host+nubo, playbook.yml

you may see 'runit' which will do all the hosts in our standard 'stack'
(e.g. stack-sde, stack-spb, stack-pts)
